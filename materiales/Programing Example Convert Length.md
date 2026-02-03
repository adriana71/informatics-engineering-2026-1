## Programing Example: Convert Length

Write a program that takes as input given lengths expressed in feet and inches. The
program should then convert and output the lengths in centimeters. Assume that the
lengths given in feet and inches are integers.

**Input:** Length in feet and inches

**Output:** Equivalent length in centimeters

#Problem Analysis and Algorith Design

The lengths are given in feet and inches, and you need to find the equivalent length in
centimeters. One inch is equal to ```2.54``` centimeters. The first thing the program needs
to do is convert the length given in feet and inches to all inches. To convert the length
from feet and inches to inches, you multiply the number of feet by ```12``` (1 foot is equal to
12 inches), and add your answer to the given inches. Then you can use the conversion
formula, 1 inch = ```2.54``` centimeters, to find the equivalent length in centimeters.
Suppose the input is 5 feet and 7 inches. You find the total inches as follows:
```
totalInches = (12 * feet) + inches
= 12 * 5 + 7
= 67
```
You can then apply the conversion formula, 1 inch = 2.54 centimeters, to find the
length in centimeters.
```
centimeters = totalInches * 2.54
= 67 * 2.54
= 170.18
```
Based on this analysis, you can design an algorithm as follows:
  1. Get the length in feet and inches.
  2. Convert the length into total inches.
  3. Convert total inches into centimeters.
  4. Output centimeters.

# Variables

The input for the program is two numbers: one for feet and one for inches. Thus,
you need two variables: one to store feet and the other to store inches. Because the
program will first convert the given length into inches, you need a third variable to
store the total inches. You need a fourth variable to store the equivalent length in
centimeters. In summary, you need the following variables:
```
  int feet; //variable to store feet
  int inches; //variable to store inches
  int totalInches; //variable to store total inches

  double centimeters; //variable to store length in centimeters
```
# Named Constants

Recall that to calculate the equivalent length in centimeters, you need to multiply the
total inches by 2.54. Instead of using the value 2.54 directly in the program, you
will declare this value as a named constant. Similarly, to find the total inches, you
need to multiply the feet by 12 and add the inches. Instead of using 12 directly in the
program, you will also declare this value as a named constant. Using named constants
makes it easier to modify the program later. Because the named constants will be
placed before the method main, you must use the modifier static to declare these
named constants.
```
static final double CENTIMETERS_PER_INCH = 2.54;
static final int INCHES_PER_FOOT = 12;
```
# Main Algorithm

In the preceding sections, we analyzed the problem and determined the formulas to
perform the calculations. We also determined the necessary variables and named
constants. We can now expand the algorithm given in the section Problem Analysis
and Algorithm Design to solve the problem given at the beginning of this programming
example (converting feet and inches to centimeters).

  1. Prompt the user for the input. (Without a prompt line, the user will stare at a blank screen and not know what to do.)
  2. Get feet.
  3. Prompt the user to enter a value for inches.
  4. Get inches.
  5. Echo the input by outputting what the program read as input.
     (Without this step, after the program has executed, you will not
     know what the input was.)
  6. Find the length in inches.
  7. Output the length in inches.
  8. Convert the length to centimeters.
  9. Output the length in centimeters.
