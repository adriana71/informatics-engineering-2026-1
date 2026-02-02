# INPUTS, VARIABLES, OUTPUTS
## Inputs & Variables
This example further illustrates how assignment statements and input statements manipulate
variables. Consider the following declarations:
```
static Scanner console = new Scanner(System.in);

int firstNum;
int secondNum;
char ch;
double z;
```
Also suppose that the following statements execute in the order given:
```
  1. firstNum = 4;
  2. secondNum = 2 * firstNum + 6;
  3. z = (firstNum + 1) / 2.0;
  4. ch = 'A';
  5. secondNum = console.nextInt();
  6. z = console.nextDouble();
  7. firstNum = (int)(z) + 8;
  8. secondNum = secondNum + 1;
  9. ch = console.next().charAt(0);
  10. firstNum = firstNum + (int)(ch);
```
In addition, suppose the input is:
```
8  16.3  D
```
Let’s now determine the values of the declared variables after the last statement executes. To show explicitly how a particular statement changes the value of a variable, the values of the variables after each statement executes are shown. (In the following table, a question mark, ?, in a box indicates that the value in the box is unknown.)

<img width="616" height="519" alt="image" src="https://github.com/user-attachments/assets/34d433c6-f9f0-4be9-9f50-ebd9766cbac7" />

<img width="581" height="511" alt="image" src="https://github.com/user-attachments/assets/a74ea0bf-d7bb-47a4-b9a9-bbc4c675c50a" />

## Outputs

> [!NOTE]
> The standard output device is usually the monitor.

In Java, output on the standard output device is accomplished by using the standard
output object System.out. The object System.out has access to two methods, print
and println, to output a string on the standard output device.

The syntax to use the object ** System.out ** and the methods ** print ** and ** println ** is:

> [!TIP]
> System.out.print(expression); <br>
> System.out.println(expression); <br>
> System.out.println(); <br>

These are output statements. The expression is evaluated, and its value is printed 
at the current insertion point on the output device. After outputting the value of
expression, the method print leaves the insertion point after the last character of
the value of expression, while the method println positions the insertion point at
the beginning of the next line. Moreover


