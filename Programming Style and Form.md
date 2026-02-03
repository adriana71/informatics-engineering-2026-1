## Programming Style and Form

Every Java application program must satisfy certain language rules. It must also satisfy the
syntax rules, which, like grammar rules, tell what is correct and what is incorrect, and what is
legal and what is illegal in the language. Other . give precise meaning to the language;
that is, they support the language’s semantics.

# Syntax

As remarked earlier, the syntax rules of a language tell what is legal and what is illegal.
Errors in syntax are detected during compilation. Consider the following Java statements:

```
int x; //Line 1
int y //Line 2
double z; //Line 3

y = w + x; //Line 4
```
When these statements are compiled, compilation errors will occur. Could you say which statements will throw compilation errors?

# Use of Blanks

In Java, you use one or more blanks to separate numbers when data is input. Blanks are
also used to separate reserved words and identifiers from each other and from other
symbols. Blanks must never appear within a reserved word or identifier

# Semantics

The set of rules that gives meaning to a language is called semantics. For example, the
order-of-precedence rules for arithmetic operators are semantic rules.
If a program contains syntax errors, the compiler will warn you. What happens when a
program contains semantic errors? It is quite possible to eradicate all syntax errors in a
program and still not have it run. And if it runs, it may not do what you meant it to do.
For example, the following two expressions are both syntactically correct expressions, but
they have different meanings:
```2 + 3 * 5``` 
and:
```(2 + 3) * 5```
If you substitute one of these expressions for the other in a program, you will not get the
same results—even though the numbers are the same, the semantics are different

# Prompt lines

Part of good documentation is the use of clearly written prompts so that users will know
what to do when they interact with a program. It is frustrating for a user to sit in front of a
running program and not have the foggiest notion of whether to enter something, and if
so, what to enter. Prompt lines are executable statements that inform the user what to
do. Consider the following Java statements, in which num is an int variable:

``` System.out.println("Please enter a number between 1 and 10 and "```
```+ "then press Enter"); ```
```num = console.nextInt();```
When these two statements execute in the order given, first the output statement causes
the following line of text to appear on the screen:

```Please enter a number between 1 and 10 and then press Enter```

After seeing this line, an example of a prompt line, users know that they must enter a
number and press the **Enter** key.

In a program, whenever users must provide input, you should include the necessary
prompt lines. The prompt lines should include sufficient information about what input is
acceptable. For example, the preceding prompt line not only tells the user to input a
number, but also informs the user that the number should be between 1 and 10.

# Form and Style
You might think that Java has too many rules. However, in practice, the rules give Java a
great degree of freedom. For example, consider the following two ways of declaring
variables:
```
  int feet;
  int inch;
  double x;
  double y;
```
and:
```
  int feet; int inch;double x;double y;
```
The computer has no difficulty understanding either of these formats, but the first form is
easier for a person to read and follow.

What about blank spaces? Where are they significant and where are they meaningless?

Consider the following Java program:
```
//An improperly formatted Java program.

import java.util.*;

public class Example2_27A
{
  static Scanner console = new Scanner(System.in);
public static void main(String[] args)
{
int num; double height;
String name;
System.out.print("Enter an integer: ");
num=console.nextInt(); System.out.println();
  System.out.println("num: "+num);
System.out.print("Enter first name: ");
name=console.next();
  System.out.println();System.out.print("Enter height: ");
height = console.nextDouble(); System.out.println();
  
System.out.println("Name: "+name);System.out.println("Height: "
+height);
}}
```
This program is syntactically correct; the Java compiler would have no difficulty reading
and compiling this program. However, this program is very hard for a human to read.
The program that you write should be properly indented and formatted. Next, we
rewrite the preceding program and properly format it.

```
//Properly formatted Java program.
import java.util.*;
public class Example2_27B
{
  static Scanner console = new Scanner(System.in);

  public static void main(String[] args)
  {
    int num;
    double height;
    String name;

    System.out.print("Enter an integer: ");
    num = console.nextInt();
    System.out.println();

    System.out.println("num: " + num);

    System.out.print("Enter first name: ");
    name = console.next();
    System.out.println();

    System.out.print("Enter height: ");
    height = console.nextDouble();
    System.out.println();

    System.out.println("Name: " + name);
    System.out.println("Height: " + height);
  }
}



