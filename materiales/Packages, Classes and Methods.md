# Java Application Program
## Packages, Classes and Methods

Only a small number of operations, such as arithmetic and assignment operations, are
explicitly defined in Java. Many of the methods and identifiers needed to run a Java
program are provided as a collection of libraries, called packages. A **package** is a
collection of related classes. Moreover, every package has a name.

In Java, class is a broadly used term. The term **class** is used to create Java programs, either
application or applet; it is used to group a set of related operations; and it is used to allow
users to create their own data types. For example, there are various mathematical
operations, such as determining the absolute value of a number, determining one number
raised to the power of another number, and determining the logarithm of a number. Each
of these operations is implemented using the Java mechanism of *methods*. Think of a
*method* as a set of instructions designed to accomplish a specific task. For example, the
name of the method implementing the operation of one number raised to the power of
another number is *pow*. This and other mathematical methods are contained in the **class
Math**. The name of the package containing the class *Math* is *java.lang*.

The package *java.util* contains the class *Scanner*. This class contains the methods
*nextInt, nextDouble, next* and *nextLine* for inputting data into a program. In the
next section, you learn how class(es) are used to create a Java application program.

## Java Application Program

The basic unit of a Java program is called a class. A Java application program is, therefore, a
collection of one or more classes. Roughly speaking, a class is a collection of methods and
data members. As described in the previous section, a method is a set of instructions
designed to accomplish a specific task. Some **predefined** or **standard** methods, such as
nextInt, print, and println, are already written and are provided as part of the system.
But to accomplish most tasks, programmers must learn to write their own methods.  

One of the classes in a Java application program must have the method called main.
Moreover, there can only be one method main in a Java class

