# hello-world
startet http://mooc.fi/courses/2013/programming-part-1/ on 05.Jan2018 and use this first git repository to upload completed exercises.

The course material:

The following material is licensed under the Creative Commons BY-NC-SA license, which means that you can use it and distribute it freely so long as you do not erase the names of the original authors. If you do changes in the material and want to distribute this altered version of the material, you have to license it with a similar free license. The use of the material for commercial use is prohibited without a separate agreement.
Authors: Arto Hellas, Matti Luukkainen
Translators to English: Emilia Hjelm, Alex H. Virtanen, Matti Luukkainen, Virpi Sumu, Birunthan Mohanathas

The course is maintained by the Agile Education Research Group


The program and the source code
Source code

A computer program is composed of commands written in the source code. A computer generally runs commands in the source code from top to bottom and from left to right. Source code is saved in a textual format and will be executed somehow.
Commands

Computers execute different operations, or actions, based on the commands. For example, when printing the text "Hello world!" on the screen, it is done by the command System.out.println.

System.out.println("Hello world!");
    

The System.out.println command prints the string given inside the brackets on the screen. The suffix ln is short for the word line. Therefore, this command prints out a line. This means that after the given string has been printed, the command will also print a line break.
Compiler and interpreter

Computers do not directly understand the programming language we are using. We need a compiler between the source code and the computer. When we are programming using the command line interface, the command javac Hello.java will compile the Hello.java file into bytecode, which can be executed using the Java interpreter. To run the compiled program, you can use the command java Hello where Hello is the name of the original source code file.

When using a modern development environment (more on this later), it will take care of compiling the source code. When we choose to run the program, the development environment will compile and execute the program. All development environments compile source code while it is being written by the programmer, which means that simple errors will be noticed before executing the program.
Components of commands
Semicolon

A semicolon ; is used to separate different commands. The compiler and the interpreter both ignore line breaks in the source code, so we could write the entire program on a single line.

In the example below we will use the System.out.print command, which is similar to the System.out.println command except that it will not print a line break after printing the text.

Example of how the semicolons are used

System.out.print("Hello "); System.out.print("world");
System.out.print("!");
    

Hello world!
    

Even though neither the compiler nor the interpreter need line breaks in the source code, they are very important when considering human readers of the source code. Line breaks are required to divide source code in a clear manner. Readability of source code will be emphasized throughout this course.
Parameters (information passed to commands)

The information processed by a command are the parameters of a command. They are passed to the command by placing them between () brackets that follow the command name. For example, the System.out.print command is given the text hello as a parameter as follows: System.out.print("hello").
Comments

Comments are a useful way to make notes in the source code for yourself and others. Everything on a line after two forward slashes // is treated as a comment.
Example of using comments

// We will print the text "Hello world"
System.out.print("Hello world");

System.out.print(" and all the people of the world."); // We print more text to the same line.

// System.out.print("this line will not be executed, because it is commented out");
    

The last line of the example introduces a particularly handy use for comments: you can comment out code instead of completely deleting it if you want to temporarily try out something.
More about printing

As we can see from the examples above, there are two commands for printing.

    System.out.print prints the text without the line break at the end
    System.out.println prints the text and the line break

The printed text can contain both traditional characters and special characters. The most important special character is \n, which stands for a line break. There are also other special characters.

System.out.println("First\nSecond\nThird");
    

When executed, the example above prints:

First
Second
Third
    

Main program body

The body for a program named "Example" is as follows:

public class Example {
    public static void main(String[] args) {
        // program code
    }
}
    

The program is stored in a text file named after the program with the .java extension. For a program named Example, the file should be named Example.java.

The execution of the program begins at the part marked with the // program code comment above. During our first week of programming, we will limit ourselves to this part. When we are talking about commands such as printing, we need to write the commands into the program body. For example: System.out.print("Text to be printed");

public class Example {
    public static void main(String[] args) {
        System.out.print("Text to be printed");
    }
}
    

From this point on, the main program body will be omitted from the examples.
Getting to know your development environment

Programming these days takes place in development environments almost without exceptions. The development environment provides several tools and features to assist the programmer. Although the development environment does not write the program on behalf of the programmer, it contains several handy features such as hinting about mistakes in code and assisting the programmer to visualize the structure of the program.

In this course, we will use the NetBeans development environment. A guide for using NetBeans is available here.

Until you become familiar with NetBeans, follow the guides and steps precisely. Most of the following exercises show what needs to be printed to the screen for the program to function correctly.

Note: Do not do the exercises by writing code and then clicking the test button. You should also execute the code manually (green arrow) and observe the result on the screen. This is especially useful if an exercise fails to pass the tests.

In the following exercises, we will practice the use of NetBeans and printing of text on the screen.

Remember to read the guide on using NetBeans before you continue!

Please answer to our survey: here. It will take less than five minutes.
Name

Create a program that prints your name to the screen.

The program output should resemble the following:

Jane Doe
        

Hello world! (And all the people of the world)

Create a program that prints out the following:

Hello world!
(And all the people of the world)
        

Spruce

Create a program that prints the following:


    *
   ***
  *****
 *******
*********
    *
        

Note: You probably wrote System.out.println("...") quite a few times. Try typing only sout on an empty line in NetBeans and then press the tab key. What happened? This tip will save a lot of your time in the future!
Variables and assignment
Variables and data types

A variable is one of the most important concepts in computer programming. A variable should be imagined as a box in which you can store information. The information stored in a variable always has a type. These types include text (String), whole numbers (int), decimal numbers (double), and truth values (boolean). A value can be assigned to a variable using the equals sign (=).

int months = 12;
    

In the statement above, we assign the value 12 to the variable named months whose data type is integer (int). The statement is read as "the variable months is assigned the value 12".

The value of the variable can be appended to a string with the plus + sign as shown in the following example.

String text = "includes text";
int wholeNumber = 123;
double decimalNumber = 3.141592653;
boolean isTrue = true;

System.out.println("The variable's type is text. Its value is " + text);
System.out.println("The variable's type is integer. Its value is  " + wholeNumber);
System.out.println("The variable's type is decimal number. Its value is " + decimalNumber);
System.out.println("The variable's type is truth value. Its value is " + isTrue);
    

Printing:

The variable's type is text. Its value is includes text
The variable's type is integer. Its value is 123
The variable's type is decimal number. Its value is 3.141592653
The variable's type is truth value. Its value is true
    

A variable holds its value until it is assigned a new one. Note that the variable type is written only when the variable is first declared in the program. After that we can use the variable by its name.

int wholeNumber = 123;
System.out.println("The variable's type is integer. Its value is  " + wholeNumber);

wholeNumber = 42;
System.out.println("The variable's type is integer. Its value is  " + wholeNumber);
    

The output is:

The variable's type is integer. Its value is 123
The variable's type is integer. Its value is 42
    

Variable data types are immutable

When a variable is declared with a data type, it cannot be changed later. For example, a text variable cannot be changed into an integer variable and it cannot be assigned integer values.

String text = "yabbadabbadoo!";
text = 42; // Does not work! :(
    

Integer values can be assigned to decimal number variables, because whole numbers are also decimal numbers.

double decimalNumber = 0.42;
decimalNumber = 1; // Works! :)
    

Varying variables

The exercise file initially contains a program which prints:

Chickens:
3
Bacon (kg):
5.5
A tractor:
There is none!

In a nutshell:
3
5.5
There is none!
        

Change the program in the specified places so that it will print:

Chickens:
9000
Bacon (kg):
0.1
A tractor:
Zetor

In a nutshell:
9000
0.1
Zetor
        

Allowed and descriptive variable names

There are certain limitations on the naming of our variables. Even though umlauts, for example, can be used, it is better to avoid them, because problems might arise with character encoding. For example, it is recommended to use A instead of Ä.

Variable names must not contain certain special characters like exclamation marks (!). Space characters cannot be used, either, as it is used to separate commands into multiple parts. It is a good idea to replace the space character using a camelCase notation. Note: The first character is always written in lower case when using the camel case notation.

int camelCaseVariable = 7;
    

Variable names can contain numbers as long it does not start with one. Variable names cannot be composed solely of numbers, either.

int 7variable = 4; // Not allowed!
int variable7 = 4; // A valid, but not descriptive variable name
    

Variable names that have been defined before cannot be used. Command names such as System.out.print cannot be used, either.

int camelCase = 2;
int camelCase = 5; // Not allowed, the variable camelCase is already defined!
    

It is strongly recommended to name variables so that their purpose can be understood without comments and without thinking. Variable names used in this course must be descriptive.
Valid variable names

    lastDay = 20
    firstYear = 1952
    name = "Matti"

Invalid variable names

    last day of the month = 20
    1day = 1952
    watchout! = 1910
    1920 = 1

Calculation

The calculation operations are pretty straightforward: +, -, * and /. A more peculiar operation is the modulo operation %, which calculates the remainder of a division. The order of operations is also pretty straightforward: the operations are calculated from left to right taking the parentheses into account.

int first = 2;   // variable of whole number type is assigned the value 2
int second = 4;  // variable of whole number type is assigned the value 4
int sum = first + second;  // variable of whole number type is assigned the value of first + second
                           //     (which means 2 + 4)

System.out.println(sum); // the value of the sum of variables is printed
    

int calcWithParens = (1 + 1) + 3 * (2 + 5);  // 23
int calcWithoutParens = 1 + 1 + 3 * 2 + 5;   // 13
    

The parentheses example above can also be done step by step.

int calcWithParens = (1 + 1);
calcWithParens = calcWithParens + 3 * (2 + 5);  // 23

int calcWithoutParens = 1 + 1;
calcWithoutParens = calcWithoutParens + 3 * 2;
calcWithoutParens = calcWithoutParens + 5;      // 13
    

Calculation operations can be used almost anywhere in the program code.

int first = 2;
int second = 4;

System.out.println(first + second);
System.out.println(2 + second - first - second);
    

Floating point numbers (decimal numbers)

Calculating the division and remainder of whole numbers is a little trickier. A floating point number (decimal number) and integer (whole number) often get mixed up. If all the variables in a calculation operation are integers, the end result will also be an integer.

int result = 3 / 2;  // result is 1 (integer) because 3 and 2 are integers as well
    

int first = 3:
int second = 2;
double result = first / second;  // the result is again 1 because first and second are integers
    

The remainder can be calculated using the remainder operation (%). For example, the calculation 7 % 2 yields 1.

int remainder = 7 % 2;  // remainder is 1 (integer)
    

If either the dividend or the divisor (or both!) is a floating point number (decimal number) the end result will also be a floating point number.

double whenDividendIsFloat = 3.0 / 2;  // result is: 1.5
double whenDivisorIsFloat = 3 / 2.0;   // result is: 1.5
    

If needed, integers can be converted to floating point using the type cast operation (double) as follows:

int first = 3;
int second = 2;
double result1 = (double)first / second;  // result is: 1.5

double result2 = first / (double)second;  // result is: 1.5

double result3 = (double)(first / second);  // result is: 1
    

In the last example calculation, the result is rounded incorrectly because the calculation between the integers is done before the type cast to a floating point number.

If the quotient is assigned to a variable of integer type, the result will be an integer as well.

int integerResultBecauseTypeIsInteger = 3.0 / 2;  // quotient is automatically integer: 1
    

The next example will print "1.5" because the dividend is transformed into a floating point number by multiplying it with a floating point number (1.0 * 3 = 3.0) before the division.

int dividend = 3;
int divisor = 2;

double quotient = 1.0 * dividend / divisor;
System.out.println(quotient);
    

What does the following code print?

int dividend = 3;
int divisor = 2;

double quotient = dividend / divisor * 1.0;
System.out.println(quotient);
    

From now on, make sure that you name your variables that follow good conventions like the variables in the examples above.
Seconds in a year

Create a program that counts how many seconds there are in a year. You can assume that a year consists of 365 days (therefore the year is not a leap year).

The program should print the following:

There are X seconds in a year.
        

X should be replaced with the calculation of your program.
Concatenation or combining strings

Let us take a closer look on combining strings with the + operator.

If the + operator is used between two strings, a new string is created with the two strings combined. Note the clever use of space characters in the values of the variables below!

String greeting = "Hi ";
String name = "John";
String goodbye = ", and goodbye!";

String sentence = greeting + name + goodbye;

System.out.println(sentence);
    

Hi John, and goodbye!
    

If a string is on either side of the + operator, the other side is converted to a string and a new string is created. For example, the integer 2 will be converted into the string "2" and then combined with the other string.

System.out.println("there is an integer --> " + 2);
System.out.println(2 + " <-- there is an integer");
    

What we learned earlier about the order of operations is still valid:

System.out.println("Four: " + (2 + 2));
System.out.println("But! Twenty-two: " + 2 + 2);
    

Four: 4
But! Twenty-two: 22
    

Using this information, we can print a mix of strings and values of variables:

int x = 10;

System.out.println("variable x has the following value: " + x);

int y = 5;
int z = 6;

System.out.println("y has the value  " + y + " and z has the value " + z);
    

This program obviously prints:

variable x has the following value: 10
y has the value 5 and z has the value 6
    

Addition

Create a program to calculate the sum of two numbers. At the beginning of the program two variables are introduced and those variables hold the numbers to be summed. Feel free to use other variables if you need to.

For example, if the variables hold numbers 5 and 4, the program should output:

5 + 4 = 9
        

If the variables hold numbers 73457 and 12888, the program output should be:

73457 + 12888 = 86345
        

Multiplication

Create a program similar to the previous one except that it multiplies the two numbers instead of adding them.

For example, if the variables hold numbers 2 and 8, the program output should be:

2 * 8 = 16
        

If the variables hold numbers 277 and 111, the program output should be:

277 * 111 = 30747
        

What is the biggest multiplication that your program is able to calculate?
Reading user input

So far our programs have been rather one-sided. Next we will learn how to read input from the user. We will use a special Scanner tool to read the user input.

Let us add the Scanner to our existing main program body. Do not worry if the main program body seems obscure as we will continue to write our code in the part marked // program code.

import java.util.Scanner;

public class ProgramBody {
    public static void main(String[] args) {
        Scanner reader = new Scanner(System.in);

        // program code
    }
}
    

Reading a string

The following code reads the user's name and prints a greeting:

System.out.print("What is your name? ");
String name = reader.nextLine(); // Reads a line of input from the user and assigns it
                                 //     to the variable called name

System.out.println("Hi, " + name);
    

What is your name? John
Hi, John
    

The program above combined along with the main program body is shown below. The name of the program is Greeting, which means that it must be located in a file named Greeting.java.

import java.util.Scanner;

public class Greeting {
    public static void main(String[] args) {
        Scanner reader = new Scanner(System.in);

        System.out.print("Who is greeted: ");
        String name = reader.nextLine(); // Reads a line of input from the user and assigns it
                                         //     to the variable called name

        System.out.print("Hi " + name);
    }
}
    

When the program above is executed, you can type the input. The output tab in NetBeans (at the bottom) looks as follows when the program has finished (the user inputs the name "John").

run:
Who is greeted: John
Hi John
BUILD SUCCESSFUL (total time: 6 seconds)
    

Reading integers

Our Scanner tool is not good for reading integers, so we will use another special tool to read an integer. The command Integer.parseInt converts the string given to it into an integer. The command's parameter is given between brackets and it returns an integer that can be assigned to an integer variable.

Basically, we are joining two commands together. First we read the input as a string from the user and immediately give it to the command Integer.parseInt.

System.out.print("Type an integer: ");
int number = Integer.parseInt(reader.nextLine());

System.out.println("You typed " + number);
    

Next we will ask the user to give us his name and age. The program body is included this time.

import java.util.Scanner;

public class NameAndAgeGreeting {
    public static void main(String[] args) {
        Scanner reader = new Scanner(System.in);

        System.out.print("Your name: ");
        String name = reader.nextLine();   // Reads a line from the users keyboard

        System.out.print("How old are you: ");
        int age = Integer.parseInt(reader.nextLine()); // Reads a string variable from the keyboard and transfers it to an integer

        System.out.println("Your name is: " + name + ", and you are " + age + " years old, nice to meet you!");
    }
}
    

Summary

The program body for interaction with the user is as follows:

import java.util.Scanner;
public class ProgramName {
    public static void main(String[] args) {
        Scanner reader = new Scanner(System.in);

        // code here
    }
}
    

Reading a string:

String text = reader.nextLine();
    

Reading an integer:

int number = Integer.parseInt(reader.nextLine());
    

Adder

Create a program that asks the user for two integers and then prints their sum.

Type a number: 6
Type another number: 2

Sum of the numbers: 8
        

In this example the user input is marked in red color. From now on the red color will indicate user input in examples.
Divider

Create a program that asks the user for two integers and prints their quotient. Make sure that 3 / 2 = 1.5. If the decimal part is missing, take another look at 6.1 Floating point numbers (decimal numbers) to find the solution.

Type a number: 3
Type another number: 2

Division: 3 / 2 = 1.5
        

Calculating the circumference

The circumference of a circle is calculated using the formula 2 * pi * radius. Create a program that asks the user for the radius and then calculates the circumference using the given radius. Java already contains the value of pi in the Math.PI variable, which you can use in your calculation.

Type the radius: 20

Circumference of the circle: 125.66370614359172
        

Bigger number

Create a program that asks the user for two integers and then prints the larger of the two.

Tip: When you write Math. (that is, Math followed by a dot) in NetBeans, it shows you a bunch of available mathematical calculations. For example, Math.cos(10) calculates the cosine of the number 10. Try to find a suitable tool in Math to complete this exercise! If you cannot find anything suitable or do not know how to complete the exercise, skip the exercise for now. We will return to the matter later on.

Type a number: 20
Type another number: 14

The bigger number of the two numbers given was: 20
        

Sum of the ages

Create a program that asks for the names and ages of two users. After that the program prints the sum of their ages.

Type your name: Matti
Type your age: 14

Type your name: Arto
Type your age: 12

Matti and Arto are 26 years old in total.
        

NHL statistics, part 1

A ready-made component NHLStatistics is included along with the exercise files for this excercise. It can be used to fetch and see NHL players' score data, including their number of played games, goals, assists, points, and penalty amount.

The main program imports (i.e. enables the use of) the component by adding the following line to the beginning of the file: import nhlstats.NHLStatistics;. The next example prints the top 10 players based on points:

import java.util.Scanner;
import nhlstats.NHLStatistics;

public class Mainprogram {
    public static void main(String[] args) throws Exception {
        Scanner reader = new Scanner(System.in);

        System.out.println("Top ten by points");
        NHLStatistics.sortByPoints();
        NHLStatistics.top(10);
    }
}
        

It will print (this was the situation on the 9th of January 2012):

Top ten by points
Henrik Sedin           VAN        43 11 + 38= 49  36
Phil Kessel            TOR        41 24 + 24= 48  10
Claude Giroux          PHI        36 18 + 30= 48  16
Joffrey Lupul          TOR        41 19 + 28= 47  36
Daniel Sedin           VAN        42 18 + 29= 47  32
Steven Stamkos         TBL        40 28 + 17= 45  34
Marian Hossa           CHI        41 17 + 27= 44  14
Evgeni Malkin          PIT        33 16 + 28= 44  30
Jordan Eberle          EDM        41 17 + 26= 43   6
Jason Pominville       BUF        41 14 + 29= 43   8
        

The name, abbreviation of the club, matches played, assists, points and penalties of players are printed.

The first command NHLStatistics.sortByPoints() sorts the list of NHL players by the points they have gathered. The second command NHLStatistics.top(10); prints the ten first players from the list. Any integer can be given as a parameter.

Similarly the players can be printed ordered by the goals or assists they have made, or by penalty minutes they have been given. First, we call the command to sort the players:

NHLStatistics.sortByPoints();     // orders the players by points
NHLStatistics.sortByGoals();      // orders the players by goals
NHLStatistics.sortByAssists();    // orders the players by assists
NHLStatistics.sortByPenalties();  // orders the players by penalty minutes
        

After that the players are printed with the command top using the number of players to be printed as its parameter.

It is also possible to use the component to request the statistics of a certain player:

NHLStatistics.searchByPlayer("Jaromir Jagr");  // prints stats of Jaromir Jagr
NHLStatistics.searchByPlayer("Koivu");         // prints stats of Mikko Koivu and Saku Koivu
NHLStatistics.searchByPlayer("Teemu");         // prints stats of all players named Teemu
        

The component can also print the statistics of all players in a club:

NHLStatistics.teamStatistics("NYR");  // Statistics of New York Rangers
        

The order of the printed club statistics can be changed using a sortBy...() first.

The name of the club must be given using the official three letter abbreviation. You can check the abbreviations here . The statistics component prints a list of the available abbreviations if you request the statistics of an invalid club.
Create a program that does the following tasks into the main program body. The tasks must be done in exactly the same order as listed below. Do the tasks in the program body one after another without deleting tasks you have already done.

Note: When you first run the program, the execution might take a while because the information is downloaded from the web. Execution should be quick after the first run.

The program must do the following:

    Print the top ten players based on goals
    Print the top 25 players based on penalty amounts
    Print the statistics for Sidney Crosby
    Print the statistics for Philadelphia Flyers (abbreviation: PHI). Note in which order the players are printed in and why that might be!
    Print the players in Anaheim Ducks (abbreviation: ANA) ordered by points

After you have successfully submitted the exercise, you can play with the code as you wish!
Conditional statements and truth values

So far, our programs have progressed from one command to another in a straightforward manner. In order for the program to branch to different execution paths based on e.g. user input, we need conditional statements.

int number = 11;

if (number > 10) {
    System.out.println("The number was greater than 10");
}
    

The condition (number > 10) evaluates into a truth value; either true or false. The if command only handles truth values. The conditional statement above is read as "if the number is greater than 10".

Note that the if statement is not followed by semicolon as the condition path continues after the statement.

After the condition, the opening curly brace { starts a new block, which is executed if the condition is true. The block ends with a closing curly brace }. Blocks can be as long as desired.

The comparison operators are:

    > Greater than
    >= Greater than or equal to
    < Less than
    <= Less than or equal to
    == Equals
    != Not equal

int number = 55;

if (number != 0) {
    System.out.println("The number was not equal to 0");
}

if (number >= 1000) {
    System.out.println("The number was greater than or equal to 1000");
}

    

A block can contain any code including other if statements.

int x = 45;
int number = 55;

if (number > 0) {
    System.out.println("The number is positive!");
    if (number > x) {
        System.out.println(" and greater than the value of variable x");
        System.out.println("after all, the value of variable x is " + x);
    }
}
    

The comparison operators can also be used outside the if statements. In such case the truth value will be stored in a truth value variable.

int first = 1;
int second = 3;

boolean isGreater = first > second;
    

In the example above the boolean (i.e. a truth value) variable isGreater now includes the truth value false.

A boolean variable can be used as a condition in a conditional sentence.

int first = 1;
int second = 3;

boolean isLesser = first < second;

if (isLesser) {
    System.out.println(first + " is less than " + second + "!");
}
    

1 is less than 3!
    

Code indentation

Note that the commands in the block following the if statement (i.e. the lines after the curly brace, { ) are not written at the same level as the if statement itself. They should be indented slightly to the right. Indentation happens when you press the tab key, which is located to the left of q key. When the block ends with the closing curly brace, indentation ends as well. The closing curly brace } should be on the same level as the original if statement.

The use of indentation is crucial for the readability of program code. During this course and generally everywhere, you are expected to indent the code properly. NetBeans helps with the correct indentation. You can easily indent your program by pressing shift, alt, and f simultaneously.
else

If the truth value of the comparison is false, another optional block can be executed using the else command.

int number = 4;

if (number > 5) {
    System.out.println("Your number is greater than five!");
} else {
    System.out.println("Your number is equal to or less than five!");
}
    

Your number is equal to or less than five!
    

A positive number

Create a program that asks the user for a number and tells if the number is positive (i.e. greater than zero).

Type a number: 5

The number is positive.
        

Type a number: -2

The number is not positive.
        

Are you certain that your code is indented correctly?

Reread the section on code indentation. Observe what happens when you press shift, alt and f simultaneously! The same automatic indentation functionality can also be used using the menu bar by selecting Source and then Format.
Age of majority

Create a program that asks for the user's age and tells whether the user has reached the age of majority (i.e. 18 years old or older).

How old are you? 12

You have not reached the age of majority yet!
        

How old are you? 32

You have reached the age of majority!
        

Even or odd?

Create a program that asks the user for a number and tells whether the number is even or odd.

Type a number: 2
Number 2 is even.
        

Type a number: 7
Number 7 is odd.
        

Hint: The number's remainder when dividing by 2 tells whether the number is even or odd. The remainder can be obtained with the % operator.
else if

If there are more than two conditions for the program to check, it is recommended to use the else if command. It works like the else command, but with an additional condition. else if comes after the if command. There can be multiple else if commands.

int number = 3;

if (number == 1) {
    System.out.println("The number is one.");
} else if (number == 2) {
    System.out.println("The number is two.");
} else if (number == 3) {
    System.out.println("The number is three!");
} else {
    System.out.println("Quite a lot!");
}
    

The number is three!
    

Let us read out loud the example above: If number is one, print out "The number is one.". Otherwise if the number is two, print out "The number is two.". Otherwise if the number is three, print out "The number is three!". Otherwise print out "Quite a lot!".
Comparing strings

Strings cannot be compared using the equality operator (==). For string comparison, we use the equals. command, which is always associated with the string to compare.

String text = "course";

if (text.equals("marzipan")) {
    System.out.println("The variable text contains the text marzipan");
} else {
    System.out.println("The variable text does not contain the text marzipan");
}
    

The equals command is always attached to the string variable with a dot in between. A string variable can also be compared to another string variable.

String text = "course";
String anotherText = "horse";

if (text.equals(anotherText)) {
    System.out.println("The texts are the same!");
} else {
    System.out.println("The texts are not the same!");
}
    

When comparing strings, it is crucial to make sure that both string variables have been assigned some value. If a value has not been assigned, the program execution terminates with a NullPointerException error, which means that variable has no value assigned to it (null).
Greater number

Create a program that asks the user for two numbers and prints the greater of those two. The program should also handle the case in which the two numbers are equal.

Example outputs:

Type the first number: 5
Type the second number: 3

Greater number: 5
        

Type the first number: 5
Type the second number: 8

Greater number: 8
        

Type the first number: 5
Type the second number: 5

The numbers are equal!
        

Grades and points

Create a program that gives the course grade based on the following table.
Points 	Grade
0–29 	failed
30–34 	1
35–39 	2
40–44 	3
45–49 	4
50–60 	5

Example outputs:

Type the points [0-60]: 37

Grade: 2
        

Type the points [0-60]: 51

Grade: 5
        

Logical operations

The condition statements can be made more complicated using logical operations. The logical operations are:

    condition1 && condition2 is true if both conditions are true.
    condition1 || condition2 is true if either of the conditions are true.
    !condition is true if the condition is false.

Below we will use the AND operation && to combine two individual conditions in order to check if the value of the variable is greater than 4 and less than 11 (i.e. in the range 5 - 10).

System.out.println("Is the number between 5-10?");
int number = 7;

if (number > 4 && number < 11) {
    System.out.println("Yes! :)");
} else {
    System.out.println("Nope :(")
}
    

Is the number between 5-10?
Yes! :)
    

Next up is the OR operation ||, which will be used to check if the value is less than 0 or greater than 100. The condition evaluates to true if the value fulfills either condition.

System.out.println("Is the number less than 0 or greater than 100?");
int number = 145;

if (number < 0 || number > 100) {
    System.out.println("Yes! :)");
} else {
    System.out.println("Nope :(")
}
    

Is the number less than 0 or greater than 100?
Yes! :)
    

Now we will use the negation operation ! to negate the condition:

System.out.println("Is the string equal to 'milk'?");
String text = "water";

if (!(text.equals("milk"))) {  // true if the condition text.equals("milk") is false
    System.out.println("No!");
} else {
    System.out.println("Yes")
}
    

Is the text equal to 'milk'?
No!
    

For complicated conditions, we often need parentheses:

int number = 99;

if ((number > 0 && number < 10) || number > 100 ) {
    System.out.println("The number was in the range 1-9 or it was over 100");
} else {
    System.out.println("The number was equal to or less than 0 or it was in the range 10-99");
}
    

The number was equal to or less than 0 or it was in the range 10-99
    

Age check

Create a program that asks for the user's age and checks that it is reasonable (at least 0 and at most 120).

How old are you? 10
OK
        

How old are you? 55
OK
        

How old are you? -3
Impossible!
        

How old are you? 150
Impossible!
        

Usernames

Create a program that recognizes the following users:
Username 	Password
alex 	mightyducks
emily 	cat

The program should check for the username and password as follows:

Type your username: alex
Type your password: mightyducks
You are now logged into the system!
        

Type your username: emily
Type your password: cat
You are now logged into the system!
        

Type your username: emily
Type your password: dog
Your username or password was invalid!
        

Note: Remember that you cannot compare strings with the == operation!
Leap year

A year is a leap year if it is divisible by 4. But if the year is divisible by 100, it is a leap year only when it is also divisible by 400.

Create a program that checks whether the given year is a leap year.

Type a year: 2011
The year is not a leap year.
        

Type a year: 2012
The year is a leap year.
        

Type a year: 1800
The year is not a leap year.
        

Type a year: 2000
The year is a leap year.
        

Introduction to loops

Conditional statements allow us to execute different commands based on the conditions. For example, we can let the user login only if the username and password are correct.

In addition to conditions we also need repetitions. We may, for example, need to keep asking the user to input a username and password until a valid pair is entered.

The most simple repetition is an infinite loop. The following code will print out the string I can program! forever or "an infinite number of times":

while (true) {
    System.out.println("I can program!");
}
    

In the example above, the while (true) command causes the associated block (i.e. the code between the curly braces {}) to be looped (or repeated) infinitely.

We generally do not want an infinite loop. The loop can be interrupted using e.g. the break command.

while (true) {
    System.out.println("I can program!");

    System.out.print("Continue? ('no' to quit)? ");
    String command = reader.nextLine();
    if (command.equals("no")) {
        break;
    }
}

System.out.println("Thank you and see you later!");
    

Now the loop progresses like this: First, the program prints I can program!. Then, the program will ask the user if it should continue. If the user types no, the break command is executed and the loop is interrupted and Thank you and see you again! is printed.

I can program!
Continue? ('no' to quit)?yeah
I can program!
Continue? ('no' to quit)? jawohl
I can program!
Continue? ('no' to quit)? no
Thank you and see you again!
    

Many different things can be done inside a loop. Next we create a simple calculator, which performs calculations based on commands that the user enters. If the command is quit, the break command will be executed to end the loop. Otherwise two numbers are asked. Then, if the initial command was sum, the program calculates and prints the sum of the two numbers. If the command was difference, the program calculates and prints the difference of the two numbers. If the command was something else, the program reports that the command was unknown.

System.out.println("welcome to the calculator");

while (true) {
    System.out.print("Enter a command (sum, difference, quit): ");
    String command = reader.nextLine();
    if (command.equals("quit")) {
        break;
    }

    System.out.print("enter the numbers");
    int first = Integer.parseInt(reader.nextLine());
    int second = Integer.parseInt(reader.nextLine());

    if (command.equals("sum") ) {
        int sum = first + second;
        System.out.println( "The sum of the numbers is " + sum );
    } else if (command.equals("difference")) {
        int difference = first - second;
        System.out.println("The difference of the numbers is " + difference);
    } else {
        System.out.println("Unknown command");
    }

}

System.out.println("Thanks, bye!");
    

Password

In this exercise we create a program that asks the user for a password. If the password is right, a secret message is shown to the user.

Type the password: turnip
Wrong!
Type the password: beetroot
Wrong!
Type the password: carrot
Right!

The secret is: jryy qbar!
        

The program will be done in three steps.
Asking for the password

The initial exercise template defines the variable String password with a value of carrot. Do not change this password! You should make the program ask the user to enter a password and then compare it with the value in the variable password. Remember what that there is a special way to compare strings!

Type the password: turnip
Wrong!
        

Type the password: carrot
Right!
        

Type the password: potato
Wrong!
        

Asking for the password until the user gives the correct one

Modify the program so that it asks the user to type a password until it gets the correct one. Implement this using a while-true loop statement. The loop statement can be interrupted if and only if the entered password matches the value of the password variable.

Type the password: turnip
Wrong!
Type the password: beetroot
Wrong!
Type the password: carrot
Right!
        

Secret message

Add your own secret message to the program and show it to the user when the password is correct. Your message can be whatever you want!

Type the password: turnip
Wrong!
Type the password: rutabaga
Wrong!
Type the password: carrot
Right!

The secret is: jryy qbar!
        

The secret above has been encrypted using the Rot13 algorithm. During this course we will implement our own encryption program.
Temperatures

You will get the Graph component along with the exercise template. Graph draws graphs based on numbers that are given to it. You can give it numbers as follows:

Graph.addNumber(13.0);
        

We will create a program that draws a graph based on daily temperatures given to it.
Asking for numbers

Create a program that asks the user to input floating point numbers (double) and then adds the numbers to the graph. Use the while-true structure again.

Note: To read a double, use: double number = Double.parseDouble(reader.nextLine());
Checking

Improve your program so that temperatures below -30 degrees or over +40 degrees are ignored and not added to the graph.
NHL statistics, part 2

We will continue using the NHL component introduced earlier and create a program that the user can use to query for statistics.

The program is structured similarly to the Calculator example program above. The program body is as follows:

public static void main(String[] args) throws Exception {
    Scanner reader = new Scanner(System.in);

    System.out.println("NHL statistics service");
    while (true) {
        System.out.println("");
        System.out.print("command (points, goals, assists, penalties, player, club, quit): ");
        String command = reader.nextLine();

        if (command.equals("quit")) {
            break;
        }

        if (command.equals("points")) {
            // print the top ten playes sorted by points
        } else if (command.equals("goals")) {
            // print the top ten players sorted by goals
        } else if (command.equals("assists")) {
            // print the top ten players sorted by assists
        } else if (command.equals("penalties")) {
            // print the top ten players sorted by penalties
        } else if (command.equals("player")) {
            // ask the user for the player name and print the statistics for that player
        } else if (command.equals("club")) {
            // ask the user for the club abbreviation and print the statistics for the club
            // note: the statistics should be sorted by points
            //     (players with the most points are first)
        }
    }
}
        

The program asks the user to give commands and then executes the operation that is associated with the given command. The commands are: points, goals, assists, penalties, player, club, quit.

You should write code in the parts marked with comments.

Here is an example demonstrating the program in action:

NHL statistics service

command (points, goals, assists, penalties, player, club): assists
Henrik Sedin           VAN        43 11 + 38= 49  36
Erik Karlsson          OTT        43  6 + 35= 41  24
Claude Giroux          PHI        36 18 + 30= 48  16
Pavel Datsyuk          DET        41 13 + 30= 43  10
Brian Campbell         FLA        42  3 + 30= 33   4
Daniel Sedin           VAN        42 18 + 29= 47  32
Jason Pominville       BUF        41 14 + 29= 43   8
Nicklas Backstrom      WSH        38 13 + 29= 42  22
Joffrey Lupul          TOR        41 19 + 28= 47  36
Evgeni Malkin          PIT        33 16 + 28= 44  30

command (points, goals, assists, penalties, player, club): player
which player: Jokinen
Olli Jokinen           CGY        43 12 + 21= 33  32
Jussi Jokinen          CAR        40  4 + 19= 23  30

command (points, goals, assists, penalties, player, club): club
which club: DET
Pavel Datsyuk          DET        41 13 + 30= 43  10
Johan Franzen          DET        41 16 + 20= 36  34
Valtteri Filppula      DET        40 14 + 21= 35  10
Henrik Zetterberg      DET        41  8 + 24= 32  14
// and more players

command (points, goals, assists, penalties, player, club): quit
        

Note: When you first run the program, the execution might take a while because the information is downloaded from the internet. Execution should be quick after the first run.

-------------------------------------------------------------------------------------------------------------------------------


Changing variables

We usually want to change the value of an existing variable. This can be done using the normal assignment statement. In the next example, we increase the value of the variable age by one:

int age = 1;

System.out.println(age);  // prints 1
age = age + 1;            // the new value of age is the old value of age + 1
System.out.println(age);  // prints 2
    

The age = age + 1 statement increments the value of the variable age by one. It is also possible to increment a variable by one as bellow:

int age = 1;

System.out.println(age);  // prints 1
age++;                    // means the same as age = age + 1
System.out.println(age);  // prints 2
    

Another example:

int length = 100;

System.out.println(length);  // prints 100
length = length - 50;
System.out.println(length);  // prints 50
length = length * 2;
System.out.println(length);  // prints 100
length = length / 4;
System.out.println(length);  // prints 25
length--;                    // means the same as length = length - 1;
System.out.println(length);  // prints 24
    

Sum of three numbers

Create a program that asks the user for three numbers and then prints their sum. Use the following structure in your program:

Scanner reader = new Scanner(System.in);
int sum = 0;
int read;

// WRITE YOUR PROGRAM HERE
// USE ONLY THE VARIABLES sum, reader AND read!

System.out.println("Sum: " + sum);
        

Type the first number: 3
Type the second number: 6
Type the third number: 12

Sum: 21
        

Sum of many numbers

Create a program that reads numbers from the user and prints their sum. The program should stop asking for numbers when user enters the number 0. The program should be structured like this:

Scanner reader = new Scanner(System.in);
int sum = 0;
while (true) {
    int read = Integer.parseInt(reader.nextLine());
    if (read == 0) {
        break;
    }

    // DO SOMETHING HERE

    System.out.println("Sum now: " + sum);
}

System.out.println("Sum in the end: " + sum);
        

The program should work as follows:

3
Sum now: 3
2
Sum now: 5
1
Sum now: 6
1
Sum now: 7
0
Sum in the end: 7
        

More loops

we have previously learned to use repetition using the while (true) loop, which repeats commands until the break command is used.

The break command is not the only way to end a loop. A common structure for a loop is while (condition), where the condition can be any statement with a truth value. This means that the condition works exactly like conditions in an if statements.

In the following example, we print the numbers 1, 2, …, 10. When the value of the variable number increases above 10, the condition of the while statement is no longer true and the loop ends.

int number = 1;

while (number < 11) {
    System.out.println(number);
    number++;  // number++ means the same as number = number + 1
}
    

The example above can be read "as long as the variable number is less than 11, print the variable and increment it by one".

Above, the variable number was incremented in each iteration of the loop. Generally the change can be anything, meaning that the variable used in the condition does not always need to be incremented. For example:

int number = 1024;

while (number >= 1) {
    System.out.println(number);
    number = number / 2;
}
    

A few programming-part1 tips

    You can find all the NetBeans tips here.
    Auto-completion of your code

    If you have, for example, the variable String familyName; in your code, you do not need to always write familyName. Try what happens when you type in f and then press CTRL and space simultaneously. You can also use auto-completion with commands like while by typing in w and then CTRL + space.
    sout

    Remember that you can get the text System.out.println("") by typing sout and pressing the tab key (located to the left of the q key)

Complete the following exercises using the while statement:
From one to a hundred

Create a program that prints the integers (whole numbers) from 1 to 100.

The program output should be:

1
2
3
(many rows of numbers here)
98
99
100
        

From hundred to one

Create a program that prints the integers (whole numbers) from 100 to 1.

The program output should be:

100
99
98
(many rows of numbers here)
3
2
1
        

Tip: Assign the variable you use in the condition of the loop a initial value of 100 and then subtract one on each iteration of the loop.
Even numbers

Create a program that prints all even numbers between 2 and 100.

2
4
6
(many rows of numbers here)
96
98
100
        

Up to a certain number

Create a program that prints all whole numbers from 1 to the number the user enters.

Up to what number? 3
1
2
3
        

Up to what number? 5
1
2
3
4
5
        

Tip: The number you read from the user now works as the upper limit in the condition of the while statement. Remember that in Java a <= b means a is less than or equal to b.
Lower limit and upper limit

Create a program that asks the user for the first number and the last number and then prints all numbers between those two.

First: 5
Last: 8
5
6
7
8
        

If the first number is greater than the last number, the program prints nothing:

First: 16
Last: 12
        

Note: Remember that the lower and upper limits can also be negative!
Assignment operations

Because changing the value of a variable is a very common operation, Java has special assignment operations for it.

int length = 100;

length += 10;  // same as length = length + 10;
length -= 50;  // same as length = length - 50;
    

When performing the assignment operation on an existing variable, it is written as variable operation= change, for example variable += 5. Note that a variable must be defined before you can assign a value to it. Defining a variable is done by specifying the variable type and the name of the variable.

The following example will not work because the type of the variable length has not been defined.

length = length + 100;  // error!
length += 100;          // error!
    

When the type is defined, the operations will also work.

int length = 0;
length = length + 100;
length += 100;

// the variable length now holds the value 200
    

There are also other assignment operations:

int length = 100;

length *= 10;   // same as length = length * 10;
length /= 100;  // same as length = length / 100;
length %= 3;    // same as length = length % 3;

// the variable length now holds the value 1
    

Often during a loop, the value of a variable is calculated based on repetition. The following program calculates 3*4 somewhat clumsily as the sum 3+3+3+3:

int result = 0;

int i = 0;
while (i < 4) {
   result = result + 3;
   i++;  // means the same as i = i + 1;
}
    

In the beginning result = 0. During the loop, the value of the variable is incremented by 3 on each iteration. Because there are 4 iterations, the value of the variable is 3*4 in the end.

Using the assignment operator introduced above, we can achieve the same behavior as follows:

int result = 0;

int i = 0;
while (i < 4) {
   result += 3;  // this is the same as result = result + 3;
   i++;          // means the same as i = i+1;
}
    

The sum of a set of numbers

Create a program that calculates the sum 1+2+3+…+n where n is a number entered by the user.

Example outputs:

Until what? 3
Sum is 6
        

The calculation above was: 1+2+3 = 6.

Until what? 7
Sum is 28
      

The calculation above was: 1+2+3+4+5+6+7 = 28.

Hint: Create the program using the while statement. Use a helper variable in your program to remember how many times the block has been executed. Use also another helper variable to store the sum. During each execution add the value of the helper variable that counts the executions to the variable in which you should collect the sum.
The sum between two numbers

Similar to the previous exercise, except that the program should ask for both the lower and upper bound. You can assume that the users first gives the smaller number and then the greater number.

Example outputs:

First: 3
Last: 5
The sum 12
    

First: 2
Last: 8
The sum is 35
    

Factorial

Create a program that calculates the factorial of the number n. The factorial n! is calculated using the formula 1*2*3*...*n. For example 4! = 1*2*3*4 = 24. Additionally, it is defined that 0! = 1.

Example outputs:

Type a number: 3
Factorial is 6
    

Type a number: 10
Factorial is 3628800
    

Sum of the powers

Create a program that calculates the sum of 20+21+22+...+2n, where n is a number entered by the user. The notation 2i means raising the number 2 to the power of i, for example 24 = 2*2*2*2 = 16. In Java we cannot write ab directly, but instead we can calculate the power with the command Math.pow(number, power). Note that the command returns a number of double type (i.e. floating point number). A double can be converted into the int type (i.e. whole number) as follows: int result = (int)Math.pow(2, 3). This assigns the value of 23 to variable result.

Example outputs:

Type a number: 3
The result is 15
    

Type a number: 7
The result is 255
    

Infinite loops

One of the classic errors in programming is to accidentally create an infinite loop. In the next example we try to print "Never again shall I program an eternal loop!" 10 times:

int i = 0;

while (i < 10) {
    System.out.println("Never again shall I program an eternal loop!");
}

The variable i, which determines is supposed to index the loops, is initially set to 0. The block is looped as long as the condition i < 10 is true. But something funny happens. Because the value of the variable i is never changed, the condition stays true forever.
Ending a while loop

So far, we have used the while loop with a structure similar to this:

int i = 1;
while (i < 10) {
    // Some code.
    i++;
}

With the structure above, the variable i remembers the number of times the the loop has been executed. The condition to end the loop is based on comparing the value of i.

Let us now recall how a while loop is stopped. Ending a while loop does not always need to be based on the amount of loops. The next example program asks for the user's age. If the given age is not in the range 5-85, the program prints a message and asks for the user's age again. As you can see, the condition for the while loop can be any expression that results in a boolean (truth value).

System.out.println("Type your age: ");

int age = Integer.parseInt(reader.nextLine());

while (age < 5 || age > 85) {  // age less than 5 OR greater than 85
    System.out.println("You are lying!");
    if (age < 5) {
        System.out.println("You are so young that you cannot know how to write!");
    } else if (age > 85) {
        System.out.println("You are so old that you cannot know how to use a computer!");
    }

    System.out.println("Type your age again: ");
    age = Integer.parseInt(reader.nextLine();
}

System.out.println("Your age is " + age);

The program could also have been implemented using the good old while (true) structure:

System.out.println("Type your age ");
int age;
while (true) {
    age = Integer.parseInt(reader.nextLine());

    if (age >= 5 && age <= 85) {  // age between 5 AND 85
        break;  // end the loop
    }

    System.out.println("You are lying!");
    if (age < 5) {
        System.out.println("You are so young that you cannot know how to write!");
    } else {  // that means age is over 85
        System.out.println("You are so old that you cannot know how to use a computer!");
    }

    System.out.println("Type your age again: ");
}

System.out.println("Your age is " + age);

Loops, ending and remembering

This set of exercises will form one larger program when put together. We create the program by adding features exercise by exercise. If you do not finish all the exercises you can still send them to be reviewed by the exercise robot. To do that, click the "submit" button, which has a picture of an arrow and is located on the right of the testing button. Even though the exercise robot complains about tests in the incomplete exercises, you will still get points for the parts you have completed.

Note: from now on every sub-exercise of a larger exercise (like 36.1) has the same value as an exercise without sub-exercises. It means that exercise 36 as a whole corresponds to five normal exercises.
Reading numbers

Create a program that asks the user to input numbers (integers). The program prints "Type numbers” until the user types the number -1. When the user types the number -1, the program prints "Thank you and see you later!" and ends.

Type numbers:
5
2
4
-1
Thank you and see you later!
    

The sum of the numbers

Develop your number reading program by adding the following feature: the program should print the sum of the numbers entered by the user (without the number -1).

Type numbers:
5
2
4
-1
Thank you and see you later!
The sum is 11
    

Summing and counting the numbers

Develop your number reading and summing program by adding the following feature: the program should print how many numbers the user typed (without the number -1).

Type numbers:
5
2
4
-1
Thank you and see you later!
The sum is 11
How many numbers: 3
    

Counting the average

Develop your number reading, summing and counting program by adding the following feature: the program should print the average of the numbers the user typed (without the number -1).

Type numbers:
5
2
4
-1
Thank you and see you later!
The sum is 11
How many numbers: 3
Average: 3.666666666666
    

Even and odd numbers

Develop your program by adding the following feature: the program should print the number of even and odd numbers that the user typed (without the number -1).

Type numbers:
5
2
4
-1
Thank you and see you later!
The sum is 11
How many numbers: 3
Average: 3.666666666666
Even numbers: 2
Odd numbers: 1
    

Note: creating a program in small steps

In these exercises we actually created one single program, but programming happened in very small steps. This is ALWAYS the preferred way to program.

When you are programming something, no matter if it is an exercise or a project of your own, it is advised to do it in very tiny pieces. Do not ever try to solve the whole problem in one go. Start with something easy, something you know that you can do. In this recent set of exercises, for example, we focused first on stopping the program when the user types -1. When one part of the program is complete and working, we can move on to work out the solution for the next sub-problem of the big main problem.

Some of the exercises in this course are sliced into smaller pieces like the set of exercises we just introduced. Usually the pieces need to be sliced again into smaller pieces depending on the problem. It is advised that you execute the whole program after almost every new line of code you write. This enables you to be sure that your solution is going in the right and working direction.
Methods

We have so far used many different commands of Java: assignment, calculations, comparison, if structures and while structures. We have been using a "command" System.out.println() to print text. We can also count the maximum of two numbers with the help of the "command" Math.max(). We are also familiar with reader.nextLine(), usually seen together with Integer.parseInt().

If we take a closer look, we notice that those commands differ from if and while (etc). The first difference is that after the command there are brackets () and sometimes an input for the command inside those brackets. Actually, the commands ending with brackets are not called commands, but methods.

Technically speaking, a method is a piece of code that can be called from different places of the program code. The line of code System.out.println("I am a parameter given to the method!") means that we call a method that actually handles the printing. After the method has been executed we go back to where we called the method, and continue executing. The input given to the method inside the brackets is called a method parameter.

In addition to a parameter, the method can also have a return value, for example, a familiar line of code:

int number = Integer.parseInt( reader.nextLine() );

includes two method calls. First the inner method reader.nextLine is called. That method has the integer typed by the user as a return value. Next the outer method Integer.parseInt is called. As a parameter for that method there is the string of characters that was received from the reader.nextLine method as a return value. The return value for the method Integer.parseInt is the string of characters transformed into an integer (whole number).

Method names also seem to include a dot, for example reader.nextLine(). Actually the method name starts after the dot, here it is nextLine(). The first part of the command that comes before the dot shows whose method is in question. Here the method belongs to the reader, which means that we have the reader's method nextLine. Later we will learn more precisely about the owner of the method (or the name on the left side of the dot). An attentive reader will notice that the method System.out.println() has two dots. Here, the method name is println and System.out is the owner of the method. Roughly System.out means the computer monitor.

This far we have been using ready-made methods from Java libraries. Next we will learn how to create our own methods.
Self-written methods

This far we have been using a programming style where code is written (and read and executed) from top to bottom.

It was mentioned before that "a method is a piece of code that can be called from different places of the program code". Ready-made methods of Java have been used since our very first program.

In addition to using these ready-made methods programmers can write their own methods for programs to call. In the real world, it is really exceptional if the program does not include any self-written methods. From now on almost every program we create during this course will include self-written methods.

The methods are written in the program body outside the main's braces ( { and } ) but still inside the outermost braces, for example like this: :

import java.util.Scanner;

public class ProgramBody {
    public static void main(String[] args) {
        Scanner reader = new Scanner(System.in);
        // program code
    }

    // self-written methods
}

Let us create a method greet.

public static void greet() {
    System.out.println("Greetings from the world of methods!");
}

And let us place it in the right spot.

import java.util.Scanner;

public class ProgramBody {
    public static void main(String[] args) {
        Scanner reader = new Scanner(System.in);
        // program code
    }

    // self-written methods
    public static void greet() {
        System.out.println("Greetings from the world of methods!");
    }
}

In order to define a new method we need to write two things. In the first row of the method definition, you will find the name of the method, in this case greet. On the left side of the name you will find the definitions public static void. On the next line, the code block marked by the braces ({ and }). Inside it, the method's code, or the commands that will be executed when the method is called. Our method greet only writes one line of text to the screen.

It is easy to call a self-written method. It happens by writing the method name, brackets () and a semicolon. In the next example main (or the main program) calls for our method, first once and then several times.

import java.util.Scanner;

public class ProgramBody {
    public static void main(String[] args) {
        Scanner reader = new Scanner(System.in);

        // program code
        System.out.println("Let us try if we can get to the method world:");
        greet();

        System.out.println("It seems like we can, let us try again:");
        greet();
        greet();
        greet();
    }

    // self-written methods
    public static void greet() {
        System.out.println("Greetings from the world of methods!");
    }
}

When the program is executed, we see the following output:

Let us try if we can get to the method world:
Greetings from the world of methods!
It seems like we can, let us try again:
Greetings from the world of methods!
Greetings from the world of methods!
Greetings from the world of methods!

What is noteworthy here is the execution order of the program code. The execution starts with the main program's (or main's) lines of code, from top to bottom, one by one. When the line of code to be executed happens to be a method call, the lines of code in the method block are executed again one by one. When the method block ends, the execution continues from the place where the method was called. To be exact, the execution continues from the next line after the original method call.

To be even more exact, the main program is also a method. When the program starts, the operation system calls for the main method. That means that the main method is the starting point of the program and the execution starts from the first code line of main. The program execution ends when it reaches the end of main.

From now on when we introduce methods, we will not point out that they need to be written in the right place inside the program code. For example, a method cannot be defined inside another method.
Printing out text

Create a method printText that prints the following string of characters: "In the beginning there were the swamp, the hoe and Java." and a line break.

public static void main(String[] args) {
    printText();
}

public static void printText() {
    // write your code here
}
    

The program output:

In the beginning there were the swamp, the hoe and Java.
    

Many prints

Develop the program by adding the following feature: the main program should ask the user how many times the text should be printed (meaning how many times the method is called).

public static void main(String[] args) {
    // ask the user how many times the text should be printed
    // use the while structure to call the printText method several times
}

public static void printText() {
    // write your code here
}
    

The program output:

How many?
7
In the beginning there were the swamp, the hoe and Java.
In the beginning there were the swamp, the hoe and Java.
In the beginning there were the swamp, the hoe and Java.
In the beginning there were the swamp, the hoe and Java.
In the beginning there were the swamp, the hoe and Java.
In the beginning there were the swamp, the hoe and Java.
In the beginning there were the swamp, the hoe and Java.
    

Note: you should print the assisting question How many? on its own line!
Method parameters

We can make our methods more useful by giving it parameters! Parameters are variables that we define inside brackets in the first line, just after the method name. When the method is called, the parameters are assigned values.

In the next example we define a method with a parameter, its name will be greet and its parameter will be a variable of the type String called name.

public static void greet(String name) {
    System.out.println("Hi " + name + ", greetings from the world of methods!");
}

Let us next call the greet method so that on the first try we give its parameter the value Matt and on the second try Arthur.

public static void main(String[] args) {
    greet("Matt");
    greet("Arthur");
}

Hi Matt, greetings from the world of methods!
Hi Arthur, greetings from the world of methods!

More complicated expressions can also be used as a parameter for our self-written methods, the same way we used them together with the ready-made System.out.println() method.

public static void main(String[] args) {
    String name1 = "Anne";
    String name2 = "Green";
    greet( name1 + " " + name2 );

    int age = 24;
    greet("John " + age + " years");
}

Hi Anne Green, greetings from the world of methods!
Hi John 24 years, greetings from the world of methods!

In both cases the method has only one parameter. The value for the parameter is calculated before calling the method. In the first case the parameter value comes from the String concatenation (a cool word that means putting the text together) name1 + " " + name2. The value for the concatenation is Anne Green. In the second case we get the parameter value from the String concatenation "John " + age + " years".
Many parameters

A method can be defined to have more than one parameter. In this case, the parameters are always listed in the same order.

public static void greet(String name, String greetingsFrom) {
    System.out.println("Hi " + name + ", greetings from " + greetingsFrom);
}

String who = "Matt";
String greetings = "Alabama";

greet(who, greetings);
greet(who, greetings + " from Nevada");

In the last greet function (or method) call the second parameter is formed by concatenating (or adding) the text “from Nevada” to the variable greetings. This is done before the actual function call.

Hi Matt, greetings from Alabama
Hi Matt, greetings from Alabama from Nevada

Method calling another method

Methods can also be called outside of main. Methods can call each other! Let us create a method greetManyTimes that greets the user many times getting assistance from the method greet:

public static void greet(String name) {
    System.out.println("Hi " + name + ", greetings from the world of methods!");
}

public static void greetManyTimes(String name, int times) {
    int i = 0;
    while ( i < times ) {
        greet(name);
        i++;
    }

}

public static void main(String[] args) {
    greetManyTimes("Anthony", 3);
    System.out.println("and");
    greetManyTimes("Martin", 2);
}

Output:

Hi Anthony, greetings from the world of methods!
Hi Anthony, greetings from the world of methods!
Hi Anthony, greetings from the world of methods!
and
Hi Martin, greetings from the world of methods!
Hi Martin, greetings from the world of methods!

Printing
Printing stars

Create a method printStars that prints the given amount of stars and a line break.

Create the method in the following body:

private static void printStars(int amount) {
    // you can print one star with the command
    // System.out.print("*");
    // call this command amount times
}

public static void main(String[] args) {
    printStars(5);
    printStars(3);
    printStars(9);
}
    

The program output:

*****
***
*********
    

Note: you can return exercises that contain many parts to the exercise robot even though you are not finished with all parts. In that case, the robot complains about tests in the unfinished parts of the exercise, but gives you points for all tests that pass.
Printing a square

Create a method printSquare(int sideSize) that prints a square using our previous method printStars. The method call printSquare(4), for example, prints the following:

****
****
****
****
    

Note: in order to complete the exercise it is not enough that the outprint looks good. Inside the printSquare method the printing must be done using the printStars method.

When you are in the middle of making your program, you should verify the correctness of your methods by writing some test code into your main method.
Printing a rectangle

Create a method printRectangle(int width, int height) that prints a rectangle using the printStars method. The call printRectangle(17,3), for example, has the following output:

*****************
*****************
*****************
    

Printing a left-aligned triangle

Create the method printTriangle(int size) that prints a triangle using the printStars method. The method call printTriangle(4), for example, has the following output:

*
**
***
****
    

Printing Like A Boss
Printing stars and whitespaces

Create a method printWhitespaces(int size) that prints the given amount of whitespaces. Them method should not print a line break.

Reimplement or copy the method printStars(int size) from the previous exercise.
Printing a right-aligned triangle

Create the method printTriangle(int size) that prints a triangle using the mehtods printWhitespaces and printStars. Note: do not print anything in the method itself, just call the helper methods to do the actual printing.

For example, the method call printTriangle(4) has the following output:

   *
  **
 ***
****
    

Printing a Christmas tree

Create the method xmasTree(int height) that prints a Christmas tree using the mehtods printWhitespaces and printStars. A Christmas tree consists of a triangle of given height and a stand. The stand is two stars tall and three stars wide and it is located in the center of the bottom of the triangle. Note: do not print anything in the method itself, just call the helper methods to do the actual printing.

The method call xmasTree(4), for example, has the following output:

   *
  ***
 *****
*******
  ***
  ***
    

The method call xmasTree(10) has the following output:

         *
        ***
       *****
      *******
     *********
    ***********
   *************
  ***************
 *****************
*******************
        ***
        ***
    

Second note: You don't need to worry about heights below 3!
Guessing a number game

In this exercise the following game is created:

Guess a number: 73
The number is lesser, guesses made: 1
Guess a number: 22
The number is greater, guesses made: 2
Guess a number: 51
The number is greater, guesses made: 3
Guess a number: 62
The number is greater, guesses made: 4
Guess a number: 68
The number is greater, guesses made: 5
Guess a number: 71
The number is lesser, guesses made: 6
Guess a number: 70
Congratulations, your guess is correct!
    

Guessing a number

The program that comes with the exercise contains a command called drawNumber. It draws a number, which is in the range 0 to 100 (both 0 and 100 are possible). Create a program that draws a number. Then the user has the chance to guess once, what the number is. The program should to print "The number is lesser", "The number is greater" or "Congratulations, your guess is correct!" depending on the number the user typed.

Guess a number: 12
The number is greater
    

Guess a number: 66
The number is lesser
    

Guess a number: 42
Congratulations, your guess is correct!
    

Repeated guessing

Develop your program by adding the following functionality: the guessing should be made repeatedly until the user types the right number. Note that you need to draw the number by using the drawNumber command before the repetition. Why? What happens if you draw the number inside the repetition?

In the example below, the command call drawNumber returned the value 83.

Guess a number: 55
The number is greater
Guess a number: 85
The number is lesser
Guess a number: 77
The number is greater
Guess a number: 81
The number is greater
Guess a number: 83
Congratulations, your guess is correct!
    

Counting the guesses

Develop your program by adding the following functionality: the program needs to include a variable of type int, which is used to count the guesses the user has made. The program should always print the number of guesses along with the answer.

Guess a number: 55
The number is greater, guesses made: 1
Guess a number: 85
The number is lesser, guesses made: 2
Guess a number: 77
The number is greater, guesses made: 3
Guess a number: 81
The number is greater, guesses made: 4
Guess a number: 83
Congratulations, your guess is correct!
    

A text-based user interface for the Hangman game

Your friend has programmed a Hangman game for you, but the game lacks the user inferface. The Hangman has the following methods:

    hangman.gameOn()
    Shows if the game is on
    hangman.printStatus()
    Prints the game status. Shows how many guesses have been made and the letters that have not been used yet.
    hangman.printWord()
    Prints the word the user tries to guess. The letters that have not been guessed yet are hidden as question marks, like "v?ri?ble".
    hangman.printMan()
    Prints the Hangman.
    hangman.guess(String letter)
    Guesses the letter that is given as a parameter.

You will get a program body from the exercise robot. It already contains some functionalities:

        Scanner reader = new Scanner(System.in);
        Hangman hangman = new Hangman();

        System.out.println("************");
        System.out.println("* Hangman *");
        System.out.println("************");
        System.out.println("");
        printMenu();
        System.out.println("");

        // ADD YOUR IMPLEMENTATION HERE

    System.out.println("Thank you for playing!");
    

In addition to the program body, you will get the method called printMenu:

    public static void printMenu() {
        System.out.println(" * menu *");
        System.out.println("quit   - quits the game");
        System.out.println("status  - prints the game status");
        System.out.println("a single letter uses the letter as a guess");
        System.out.println("an empty line prints this menu");
    }
    

The exercise is completed in small steps.
Loops and ending loops

Create a loop in the program that works as a base for the rest of the user interface. Ask the user to submit the command inside the loop. If the command is "quit", break the loop.

Use the command hangman.gameOn as the condition for the while structure. The loop should look like:

while (hangman.gameOn()) {
    String command = reader.nextLine();
    // ...
}
    

In the next set (week) of exercises, we will find out what this peculiar-looking condition for ending the loop is about.

This far the program should produce the following output:

************
* Hangman *
************

 * menu *
quit   - quits the game
status - prints the game status
a single letter uses the letter as a guess
an empty line prints this menu

Type a command:
do not quit

Type a command:
quit
Thank you for playing!
    

Printing the status

If the user gives the command "status", print the status using the method hangman.printStatus().

************
* Hangman *
************

* menu *
quit   - quits the game
status - prints the game status
a single letter uses the letter as a guess
an empty line prints this menu

Type a command:
status
You have not made any guesses yet.
Unused letters: abcdefghijklmnopqrstuvwxyz

Type a command:
quit
Thank you for playing!
    

Making a guess

If the user types in a single letter as a command, use it to make a guess. Guessing a letter occurs in the method hangman.guess(command). The guessing command has its own printing functionality, which it uses to print more information about the guess.

Hint: finding out if the command is a single letter is done as follows:

String command = reader.nextLine();

if(command.length() == 1) {  // command has only one letter, so it must be a guess
    hangman.guess(command);
}
    

...
Type a command:
a
The letter a is not in the word.

Type a command:
b
The letter b is not in the word.

Type a command:
c
The letter c was found in the word!

Type a command:
quit
Thank you for playing!
    

Printing out the menu

If the user types an empty string of characters, meaning a string that has zero length, you need to call the method printMenu. Note that the method printMenu is not in the Hangman game but in your own program.

Note: checking if the string is empty is done as follows:

String winnie = "the pooh";
if(winnie.isEmpty()) {
    System.out.println("String was empty");
} else {
    System.out.println("I found something!");
}
    

Printing the man and the word

If the user has not typed the command quit, you should call the Hangman game commands hangman.printMan() and hangman.printWord() at the end of the loop.

...
Type a command:
a
The letter a is not in the word.
 ____
 |
 |
 |
 |
/|\
Word to be guessed: ????

Type a command:
m
The letter m was found in the word!
 ____
 |
 |
 |
 |
/|\
Word to be guessed: m???

Type a command:
quit
Thank you for playing!
    

-------------------------------------------------------------------------------------------------------------------------------


More about methods
Methods and visibility of variables

Let us try to change from within a method the value of a variable located in the main program.

// main program
public static void main(String[] args) {
    int number = 1;
    addThree();
}

// method
public static void addThree() {
    number = number + 3;
}

Unfortunately this program will not work, because the method cannot "see" the variable number located in the main program.

This holds generally. Variables defined in the main program are not visible for other methods. Also, the other way is similar: variables defined in methods are not visible for other methods or the main program. The only way to give information to a method from the outside is to use parameters.

// main program
public static void main(String[] args) {
    int number = 1;
    System.out.println("Main program variable number holds the value: " + number);
    addThree(number);
    System.out.println("Main program variable number holds the value: " + number);
}

// method
public static void addThree(int number) {
    System.out.println("Method parameter number holds the value: " + number);
    number = number + 3;
    System.out.println("Method parameter number holds the value: " + number);
}

In the program above the method addThree has a parameter called number. This parameter is copied (duplicated) for the method to use. When the program above is executed we see the following output:

Main program variable number holds the value: 1
Method parameter number holds the value: 1
Method parameter number holds the value: 4
Main program variable number holds the value:  1

The number we gave as a parameter to the method was copied for the method to use. If we would like the main program to be able to use the new value generated by the method, the method needs to return that value.
Return values

A method can return a value. In the examples above, methods have not been returning anything. This is expressed by writing void in the first line of the method, just before it's name.

public static void addThree() {
  ...

When defining a method that returns a value, we also have to define the type of the return value. We can define the type of the return value by writing it just before the name of the method. Next, we have a method that always returns the number 10 (type int). Returning a value is accomplished with the command return:

public static int alwaysReturnTen() {
    return 10;
}

If we want to use the returned value later, we have to catch the return value and store it into a variable:

public static void main(String[] args) {
    int number = alwaysReturnTen();

    System.out.println( "method returned the number " + number );
}

The return value of the method is assigned to a variable of type int just like any other integer. The return value can also be a part of a sentence:

double number = 4 * alwaysReturnTen() + (alwaysReturnTen() / 2) - 8;

System.out.println( "calculation total " + number );

Every variable type we have seen this far can be used as a return value:

public static void methodThatReturnsNothing() {
  // method body
}

public static int methodThatReturnsInteger() {
  // method body, needs a return statement
}

public static String methodThatReturnsText() {
  // method body, needs a return statement
}

public static double methodThatReturnsFloatingpoint() {
  // method body, needs a return statement
}

If the method is defined to have a return value, it also has to return a value. The following method is incorrect:

public static String wrongMethod() {
    System.out.println("I tell you that I will return a String but I do not!");
}

In the following example, we define a method for calculating a sum. Then, we use the method to calculate 2 + 7. The return value (returned after the method call) is assigned to a variable called sumNumbers.

public static int sum(int first, int second) {
    return first + second;
}

Method call:

int sumNumbers = sum(2, 7);
// sumNumbers now holds the value 9

Let us expand the example program so that the user types the numbers.

public static void main(String[] args) {
    Scanner reader = new Scanner(System.in);

    System.out.print("Type the first number: ");
    int first = Integer.parseInt( reader.nextLine() );

    System.out.print("Type the second number: ");
    int second = Integer.parseInt( reader.nextLine() );

    System.out.print("Total: " + sum(first,second) );
}

public static int sum(int first, int second) {
    return first + second;
}

As we can see, the return value of the method does not always need to be assigned to a variable. It can also act as a part of the printing command just like any other integer value.

In the next example, we call the method sum using integers that we get as return values from the method sum.

int first = 3;
int second = 2;

sum(sum(1, 2), sum(first, second));
// 1) the inner methods are executed:
//    sum(1, 2) = 3   and sum(first, second) = 5
// 2) the outer method is executed:
//    sum(3, 5) = 8

The method's own variables

The following method calculates the average of the numbers the method gets as parameters. The method uses helper variables sum and average. The method's own variables can be introduced just like any other variables.

public static double average(int number1, int number2, int number3) {

    int sum = number1 + number2 + number3;
    double average = sum / 3.0;

    return average;
}

Sum of numbers

Create the method sum that calculates the sum of numbers the method receives as parameters.

Place the method in the following program body:

public static int sum(int number1, int number2, int number3, int number4) {
    // write program code here
    // remember that the method needs a return in the end
}

public static void main(String[] args) {
    int answer = sum(4, 3, 6, 1);
    System.out.println("sum: " + answer);
}
    

Example output:

sum: 14
    

Note: if an exercise involves a method returning something, it means that the return type needs to be defined for the method, and that the method needs to return a value of that type using the return command. In this case, the method does not print (or use the command System.out.println(..)), the method caller handles printing, here, the main program..
Least

Create the method least, which returns the least of the numbers given as parameters. If the parameters are equal, you can decide which one is returned.

public static int least(int number1, int number2) {
    // write program code here
    // do not print anything inside the method

    // method needs a return in the end
}

public static void main(String[] args) {
    int answer =  least(2, 7);
    System.out.println("Least: " + answer);
}
    

Example output:

Least: 2
    

Greatest

Create the method greatest, which gets three integers as parameters and then returns the greatest of them. If there are several parameters that are equally great, you can decide which one is returned. Printing should be done in the main program.

public static int greatest(int number1, int number2, int number3) {
    // write your code here
}

public static void main(String[] args) {
    int answer =  greatest(2, 7, 3);
    System.out.println("Greatest: " + answer);
}
    

Example output:

Greatest: 7
    

Average of given numbers

Create the method average, which calculates the average of the numbers it gets as parameters. Inside the method you should use the method sum as a helper!

Place the method in the following program body:

public static double average(int number1, int number2, int number3, int number4) {
    // write your code here
}

public static void main(String[] args) {
    double answer = average(4, 3, 6, 1);
    System.out.println("average: " + answer);
}

    

Program output:

average: 3.5
    

Make sure you remember how you can transform a whole number (int) into a decimal number (double)!
Strings of characters

In this section, we take a closer look at strings of characters in Java, which are called Strings. We have already used variables of String type when printing, and learned how to compare Strings. Comparing two strings is performed by calling the equals() method of the string.

String animal = "Dog";

if( animal.equals("Dog") ) {
    System.out.println(animal + " says bow-wow");
} else if ( animal.equals("Cat") ) {
    System.out.println(cat + " says meow meow");
}

It is possible to ask the string how many characters long it is by writing .length() after it's name. In other words, we are calling its length() method.

String banana = "banana";
String cucumber = "cucumber";
String together = banana + cucumber;

System.out.println("The length of banana is " + banana.length());
System.out.println("The length of  cucumber is " + cucumber.length());
System.out.println("The word " + together + " length is " + together.length());

In the above code, the method length() is called for three different strings. The call banana.length() calls only the method that gives the length of the string banana, while cucumber.length() calls the method that gives the length of the string cucumber etc. The left part before the dot says whose method is called.

Java has a special data type, called char, to be used for characters. A char variable can store only one character. A string variable can return a character from a specific location in itself with the method charAt() that uses the index of the location as a parameter. Note that counting the index of the character starts from zero!

String word = "Supercalifragilisticexpialidocious";

char character = word.charAt(3);
System.out.println("The 4th character of the word is " + character); //prints "e"

The characters in a string are numbered (indexed) starting from 0. This means that we can reach the last character in a string with number (or index) "the length of the word minus one", or word.charAt(word.length()-1). The following example will make the program crash, because we are trying to get a character from an index that does not exist.

char character = word.charAt(word.length());

A tip for using NetBeans

    You can find all the NetBeans tips here
    Renaming

    Variables, methods and classes (we will learn about these in the next set) need to have descriptive names. Often, a name is not that describing and needs to be changed. In NetBeans, it is really easy to rename things. Just select and "paint" the name you want to change with the mouse. Then press ctrl and r simultaneously, and write the new name.

The length of a name

Create a program that asks for the user's name and says how many characters the name contains.

Type your name: Paul
Number of characters: 4
    

Type your name: Catherine
Number of characters: 9
    

Note!Your program should be structured so that you put the calculating of the name length in it's own method: public static int calculateCharacters(String text). The tests will be testing both the method calculateCharacters and the program overall.
First character

Create a program that asks for the user's name and gives the first character.

Type your name: Paul
First character: P
    

Type your name: Catherine
First character: C
    

Note! Your program should be structured so that you put the search for the first character in its own method: public static char firstCharacter(String text). The tests will be testing both the method firstCharacter and the program overall
Last character

Create a program that asks for the user's name and gives the last character.

Type your name: Paul
Last character: l
    

Type your name: Catherine
Last character: e
    

Note! Your program should be structured so that you put the search for the last character in its own method: public static char lastCharacter(String text). The tests will be testing both the method lastCharacter and the program overall.
Separating first characters

Create a program that asks for the user's name and gives its first, second and third characters separately. If the name length is less than three, the program prints nothing. You do not need to create methods in this exercise.

Type your name: Paul
1. character: P
2. character: a
3. character: u
    

Type your name: me
    

Note: watch closely at the output in this and the following exercise. The print needs to contain a space after the dot and the colon!
Separating characters

Create a program that asks for the user's name and gives its characters separately. You do not need to create methods in this exercise.

Type your name: Paul
1. character: P
2. character: a
3. character: u
4. character: l
    

Hint: using a while loop helps in this exercise!

Type your name: Catherine
1. character: C
2. character: a
3. character: t
4. character: h
5. character: e
6. character: r
7. character: i
8. character: n
9. character: e
    

Reversing a name

Create a program that asks for the user's name and prints it in reverse order. You do not need to create a separate method for this.

Type your name: Paul
In reverse order: luaP
    

Type your name: Catherine
In reverse order: enirehtaC
    

Hint: You can print one character using the command System.out.print()
Other methods for strings

We often want to read only a specific part of a string. A method in the String class called substring makes this possible. It can be used in two ways:

String word = "Supercalifragilisticexpialidocious";
System.out.println(word.substring(14)); //prints "listicexpialidocious"
System.out.println(word.substring(9,20)); //prints "fragilistic"

We can store the return value in a variable, because the return value of the substring method is of type String.

String book = "Mary Poppins";
String endpart = book.substring(5);
System.out.println("Harry " + endpart); // prints "Harry Poppins"

Methods in the String class also make it possible to search for a specific word in text. For example, the word "or" can be found in the word "Horse". A method called indexOf() searches for the word given as a parameter in a string. If the word is found, it returns the starting index (location), remember that the numbering starts from 0 of the word. If the word is not found, the method returns the value -1.

String word = "aesthetically";

int index = word.indexOf("tic"); // index value will be 6
System.out.println(word.substring(index)); //prints "tically"

index = word.indexOf("ally"); //index value will be 9
System.out.println(word.substring(index)); //prints "ally"

index = word.indexOf("book"); // string "aesthetically" does not include "book"
System.out.println(index); //prints -1
System.out.println(word.substring(index)); //error!

First part

Create a program that prints the first part of a word. The program asks the user for the word and the length of the first part. Use the substring method in your program.

Type a word: example
Length of the first part: 4
Result: exam
    

Type a word: example
Length of the first part: 6
Result: exampl
    

The end part

Create a program that prints the end part of a word. The program asks the user for the word and the length of the end part. Use the substring method in your program.

Type a word: example
Length of the end part: 4
Result: mple
    

Type a word: example
Length of the end part: 6
Result: xample
    

A word inside a word

Create a program that asks the user for two words. Then the program tells if the second word is included in the first word. Use String method indexOf in your program.

Type the first word: glitter
Type the second word: litter
The word 'litter' is found in the word 'glitter'.
    

Type the first word: glitter
Type the second word: clean
The word 'clean' is not found in the word 'glitter'.
    

Note: Make your program outputs (prints) match exactly the example above!
Reversing text

Create the method reverse that puts the given string in reversed order. Use the following program body for the method:

public static String reverse(String text) {
    // write your code here
}

public static void main(String[] args) {
    System.out.print("Type in your text: ");
    String text = reader.nextLine();
    System.out.println("In reverse order: " + reverse(text));
}
    

Hint: you probably need to build the reversed string character by character in your method. You can use a String-type variable as a helper during the building process. In the beginning, the helper variable should have an empty string of characters as a value. After this, new characters are added to the string one by one.

String help = "";

// ...
// adding a character to the help variable
help = help + character;
    

Program output:

Type a text: example
elpmaxe
    

Object

Strings and integers have some differences. Integers are "just values", they can be used in calculations and they can be printed on the screen:

int x = 1;
int y = 2;

y = 3*x;

System.out.println( "value of y now: " + y );

Strings are a bit "cleverer" and for example know how long they are:

String word1 = "Programming";
String word2 = "Java";

System.out.println( "String "+ word1 +" length: " + word1.length() );

System.out.println( "String "+ word2 +" length: " + word2.length() );

Program output:

String Programming length: 11
String Java length: 4

We can determine the length by calling the String method length(). Strings have other methods as well. Integers (or whole numbers, variables of type int) have no methods at all. They do not "know" anything.

Strings are objects, or "something that has methods and a value". Later we will see many other objects as well.

As we can see in the previous example, an object's methods are called by adding a dot and a method call after the name of the object:

word1.length()    // String object's name is word1 and its method length() is called
word2.length()    // String object's name is word2 and its method length() is called

The method call is made explicitly to the object. In the above example, we have two objects and first we call the length() method of the String object word1 and then do the same for the object word2.

Our old friend reader is also an object:

Scanner reader = new Scanner(System.in);

Even though readers and strings are both objects, they are not very similar. For example, readers (Scanners) have the nextLine() method, but Strings do not. In the Java programming language, objects must be "born", in other words created with the new command. Strings are objects that make an exception to this rule! -- There are two ways to create a String object:

String banana = new String("Banana");
String carrot = "carrot";

Both of the commands above create a new String object. Using the new command when creating a String objects is uncommon.

The object's "type" is called a class. The class of a string of characters is called String and the class of readers is called Scanner. Later we learn much more about classes and objects.
ArrayList or an "object container"

Often during programming, we would like to keep many different strings in memory. A very bad idea would be to define a variable for each of them: :

String word1;
String word2;
String word3;
// ...
String word10;

This would be such a good-for-nothing solution that it does not almost need an explanation -- think of this approach for a word count of 100 or 1000!

Just like other modern programming languages, Java gives us different tools to store many objects neatly in our programs. Now, we take a closer look at ArrayList, which is probably the most used object container in Java.

The following lines of code make use of an ArrayList that holds specifically objects of type String. A couple of strings are stored into the list.

import java.util.ArrayList;

public class ListProgram {

    public static void main(String[] args) {
        ArrayList<String> wordList = new ArrayList<String>();

        wordList.add("First");
        wordList.add("Second");
    }
}

In the above main program method, the first row creates a new ArrayList called wordList, which can be used as a container for String variables. The type of the ArrayList is ArrayList<String>, which means that the ArrayList is meant for storing Strings. The list is created using the command new ArrayList<String>();.

Note: to make the ArrayList work, we must first write an import statement at the beginning of the program either import java.util.ArrayList; or import java.util.*;

When the list is created, two strings are added by calling the list method add. The list will not run out of space, so theoretically the list can contain any amount of Strings (as long as they fit in the computer's memory).

Internally an ArrayList is -- as its name suggests -- a list. The added strings automatically go to the end of the ArrayList.
Methods of ArrayLists

ArrayList provides us with many useful methods:

public static void main(String[] args) {
    ArrayList<String> teachers = new ArrayList<String>();

    teachers.add("Anthony");
    teachers.add("Barto");
    teachers.add("Paul");
    teachers.add("John");
    teachers.add("Martin");
    teachers.add("Matt");

    System.out.println("the number of teachers " + teachers.size() );

    System.out.println("first teacher on the list " + teachers.get(0));
    System.out.println("third teacher on the list " + teachers.get(2));

    teachers.remove("Barto");

    if (teachers.contains("Barto")) {
        System.out.println("Barto is on the teachers list");
    } else {
        System.out.println("Barto is not on the teachers list");
    }
}

First a list of strings is created and then 6 names added to it. size tells us the amount of strings in the list. Note: when the method is called, the call should have the following format: teachers.size(). First comes the name of the object, then follows a dot followed by the name of the method.

The strings will be in the list in the order in which they were added to it. By calling the method get(i), we get the value from the index (location) i in the list. The indexing of items in the list starts from 0. This means that the first added string is located at index 0, the second at index 1, and so on.

We can remove strings from lists through the method remove. The method can be used in two ways. First, remove("characters") removes the string given as a parameter. Second, remove(3) removes the 4th String from the list.

At the end of the example, the method contains is called. This method is used for asking the list if it contains the string given as a parameter. If it does, the method returns the value true.

Program output:

the number of teachers 6
first teacher on the list Anthony
third teacher on the list Paul
Barto is not on the teachers list

Note! The methods remove and contains assume that the objects stored in the ArrayList do have an equals method. We will get back to this later in the course.
Going through an ArrayList

In the following example 4 names are added to the list. Then the whole list is printed:

public static void main(String[] args) {
    ArrayList<String> teachers = new ArrayList<String>();

    teachers.add("Anthony");
    teachers.add("Paul");
    teachers.add("John");
    teachers.add("Martin");

    System.out.println( teachers.get(0) );
    System.out.println( teachers.get(1) );
    System.out.println( teachers.get(2) );
    System.out.println( teachers.get(3) );
}

This solution works, but is really clumsy. What if there were more items in the list? Or less? What if we would not know how many items there are?

First, we create a temporary version:

public static void main(String[] args) {
    ArrayList<String> teachers = new ArrayList<String>();

    teachers.add("Anthony");
    teachers.add("Paul");
    teachers.add("John");
    teachers.add("Martin");
    teachers.add("Matt");

    int place = 0;
    System.out.println( teachers.get(place) );
    place++;
    System.out.println( teachers.get(place) );  // place = 1
    place++;
    System.out.println( teachers.get(place) );  // place = 2
    place++;
    System.out.println( teachers.get(place) );  // place = 3
}

Using our old friend the while command, we can increment the variable place by one until it gets too big:

public static void main(String[] args) {
    ArrayList<String> teachers = new ArrayList<String>();

    teachers.add("Anthony");
    teachers.add("Paul");
    teachers.add("John");
    teachers.add("Martin");
    teachers.add("Matt");

    int place = 0;
    while ( place < teachers.size() )  // remember why place <= teachers.size() doesn't work?
        System.out.println( teachers.get(place) );
        place++;
    }
}

Now, printing works regardless of the amount of items in the list.

Using a while loop, and "self indexing" the locations in the list, is usually not the best way to go through a list. A much more recommended way is to use the for-each loop described below.
for-each

Even though the command is usually referred to as for-each, the real name of the command is only for. There are two versions of for, the traditional and the "for-each". The latter is used now.

Going through items in an ArrayList with for-each is easy:

public static void main(String[] args) {
    ArrayList<String> teachers = new ArrayList<String>();

    teachers.add("Anthony");
    teachers.add("Paul");
    teachers.add("John");
    teachers.add("Martin");
    teachers.add("Matt");

    for (String teacher : teachers) {
        System.out.println( teacher );
    }
}

As we can see, the indexes of the list can be ignored if we go through the content of the list "automatically".

In the code block of the for command (inside { }) a variable teacher is used. It is defined in the for row, on the left side of the colon. What happens is that every item in the list teachers becomes the value of the variable teacher, one by one. It means that when for is entered, the first teacher is Anthony, the second execution of for makes the teacher become Paul etc.

Even though the for command might seem a bit strange at first, you should definitely get used to use it!
Words

Create a program that asks the user to input words until the user types in an empty String. Then the program prints the words the user gave. Try the for repetition sentence here. Use an ArrayList structure in your program. ArrayList is defined like this:

ArrayList<String> words = new ArrayList<String>();
    

Type a word: Mozart
Type a word: Schubert
Type a word: Bach
Type a word: Sibelius
Type a word: Liszt
Type a word:
You typed the following words:
Mozart
Schubert
Bach
Sibelius
Liszt
    

Note: an empty String can be detected this way:

String word = reader.nextLine();

if ( word.isEmpty() ) {  // could also be: word.equals("")
   // word was empty, meaning that the user only pressed enter
}
    

Recurring word

Create a program that asks the user to input words until the user gives the same word twice. Use an ArrayList structure in your program. ArrayList is defined like this:

ArrayList<String> words = new ArrayList<String>();
    

Type a word: carrot
Type a word: celery
Type a word: turnip
Type a word: rutabaga
Type a word: celery
You gave the word celery twice
    

Hint: Remember that ArrayList has the method .contains()
Ordering, reversing and shuffling a list

Items in an ArrayList are easy to order by size. Ordering by size means an alphabetic order when the list items are of type String. Ordering is done as follows:

public static void main(String[] args) {
    ArrayList<String> teachers = new ArrayList<String>();

    // ...

    Collections.sort(teachers);

    for (String teacher : teachers) {
        System.out.println( teacher );
    }
}

Output:

Anthony
Barto
John
Martin
Matt
Paul

We give the list as a parameter for the method Collections.sort. The import line import java.util.Collections; or import java.util.*; needs to be at the beginning of the program in order to get tools of Collections working in our program.

Collections also includes other useful methods:

    shuffle shuffles the list items, can be useful for example in games
    reverse reverses the order of list items

Words in reverse order

Create a program that asks the user to input words, until the user gives an empty string. Then the program prints the words the user gave in reversed order, the last word is printed first etc.

Type a word: Mozart
Type a word: Schubert
Type a word: Bach
Type a word: Sibelius
Type a word: Liszt
Type a word:
You typed the following words:
Liszt
Sibelius
Bach
Schubert
Mozart
    

Words in alphabetical order

Create a similar program as the previous one, but in which the words are printed in alphabetical order.

Type a word: Mozart
Type a word: Schubert
Type a word: Bach
Type a word: Sibelius
Type a word: Liszt
Type a word:
You typed the following words:
Bach
Liszt
Mozart
Schubert
Sibelius
    

ArrayList as a parameter for a method

ArrayList can be given to a method as a parameter:

public static void print(ArrayList<String> list) {
    for (String word : list) {
        System.out.println( word );
    }
}

public static void main(String[] args) {
    ArrayList<String> list = new ArrayList<String>();
    list.add("Java");
    list.add("Python");
    list.add("Ruby");
    list.add("C++");

    print(list);
}

The type of the parameter is defined as an ArrayList of String variables the same way a String ArrayList is defined:

Note that the name of the parameter can be anything:

public static void print(ArrayList<String> printed) {
    for (String word : printed) {
        System.out.println( word );
    }
}

public static void main(String[] args) {
    ArrayList<String> programmingLanguages = new ArrayList<String>();
    programmingLanguages.add("Java");
    programmingLanguages.add("Python");
    programmingLanguages.add("Ruby");
    programmingLanguages.add("C++");

    ArrayList<String> countries = new ArrayList<String>();
    countries.add("Finland");
    countries.add("Sweden");
    countries.add("Norway");

    print(programmingLanguages);    // method is given the list programmingLanguages
as a parameter

   print(countries);                 //  method is given the list countries as a parameter
}

The program now includes two lists, programmingLanguages and countries. First the printing method is given the list programmingLanguages. The method print internally refers to the list given as a parameter with the name printed! Next, the printing method is given the list countries. Now, the method uses again the name printed referring to the parameter list.
Amount of items in a list

Create the method public static int countItems(ArrayList<String> list) that returns the number of the items in the list. Your method should not print anything. Use a return statement to return the number as shown in the following example:

ArrayList<String> list = new ArrayList<String>();
list.add("Hallo");
list.add("Ciao");
list.add("Hello");
System.out.println("There are this many items in the list:");
System.out.println(countItems(list));
    


There are this many items in the list:
3
    

Inside the method, it is possible to influence the items in the parameter list. In the following example, the method removeFirst --as the name suggests-- removes the first string from the list. What would happen if the list was empty?

public static void print(ArrayList<String> printed) {
    for (String word : printed) {
        System.out.println( word );
    }
}

public static void removeFirst(ArrayList<String> list) {
    list.remove(0);  // removes the first item (indexed 0)
}

public static void main(String[] args) {
    ArrayList<String> programmingLanguages = new ArrayList<String>();
    programmingLanguages.add("Pascal");
    programmingLanguages.add("Java");
    programmingLanguages.add("Python");
    programmingLanguages.add("Ruby");
    programmingLanguages.add("C++");

    print(programmingLanguages);

    removeFirst(programmingLanguages);

    System.out.println();  // prints an empty line

   print(programmingLanguages);
}
    

Output:

Pascal
Java
Python
Ruby
C++

Java
Python
Ruby
C++
    

Similarly a method could, for example, add more strings to the list it received as a parameter.
Remove last

Create the method public static void removeLast(ArrayList<String> list), which removes the last item from the list. Example code:

ArrayList<String> brothers = new ArrayList<String>();
brothers.add("Dick");
brothers.add("Henry");
brothers.add("Michael");
brothers.add("Bob");

System.out.println("brothers:");
System.out.println(brothers);

// sorting brothers
brothers.sort();

// removing the last item
removeLast(brothers);

System.out.println(brothers);
    

Example output:

brothers:
[Dick, Henry, Michael, Bob]
[Bob, Dick, Henry]
    

As we notice from the example above, an ArrayList can be printed as it is. The print formatting is not usually what is sought after, so we are forced to handle the printing ourself. For example, with the help of the for command.
Numbers in an ArrayList

ArrayLists can be used to store any type of values. If the stored variables are of integer type, there are a couple of details to remember. An integer ArrayList is defined like this: ArrayList<Integer>, instead of writing int you must write Integer.

The method remove does not work like expected when the list consists of int numbers::

public static void main(String[] args) {
    ArrayList<Integer> numbers = new ArrayList<Integer>();

    numbers.add(4);
    numbers.add(8);

    // tries to remove the number from the index 4, does not work as expected!
    numbers.remove(4);

    // this removes the number 4 from the list
    numbers.remove(Integer.valueOf(4));
}

numbers.remove(4) tries to remove the item in the index 4 from the list. There are only 2 items in the list, so the command generates an error. We must use a slightly more complicated command if the number 4 needs to be removed: numbers.remove( Integer.valueOf(4) );

ArrayLists can also be used to store doubles (decimal numbers) and characters (char variables). The lists can be defined as follows:


        ArrayList<Double> doubles = new ArrayList<Double>();
        ArrayList<Character> characters = new ArrayList<Character>();

Sum of the numbers

Create the method sum, which receives a list of numbers (ArrayList<Integer>) as a parameter and then calculates the sum of the items in that list.

Create the method using the following program body:

public static int sum(ArrayList<Integer> list) {
    // write your code here
}

public static void main(String[] args) {
    ArrayList<Integer> list = new ArrayList<Integer>();
    list.add(3);
    list.add(2);
    list.add(7);
    list.add(2);

    System.out.println("The sum: " + sum(list));

    list.add(10);

    System.out.println("the sum: " + sum(list));
}
    

Program output:


The sum: 14
The sum: 24
    

Average of numbers

Create the method average, which receives a list of numbers (ArrayList<Integer>) as a parameter and then calculates the average of the items in that list.

Note: the method should use the method sum from the previous exercise to calculate the sum of the parameters.

Create the method using the following program body:

public static double average(ArrayList<Integer> list) {
    // write your code here
}

public static void main(String[] args) {
    ArrayList<Integer> list = new ArrayList<Integer>();
    list.add(3);
    list.add(2);
    list.add(7);
    list.add(2);

    System.out.println("The average is: " + average(list));
}
    

Program output:


The average is: 3.5
    

ArrayList as return value of a method

ArrayList can also be returned from a method as a return value. In the next example, a method creates an ArrayList, adds three integers into the list and then returns the list. Pay attention to how the main program assigns the list returned by the method as a value into a variable that has the same type as the return value:

public class Main {

    public static ArrayList<Integer> addNumbersToList(int num1, int num2, int num3){
        ArrayList<Integer> list = new ArrayList<Integer>();

        list.add(num1);
        list.add(num2);
        list.add(num3);

        return list;
    }

    public static void main(String[] args) {
        ArrayList<Integer> numbers = addNumbersToList(3, 5, 2);

        for (int number : numbers) {
            System.out.println( number );
        }
    }
}

The lengths of the Strings

Create the method lengths that gets a list of String variables as a parameter and returns an ArrayList that contains the lengths of the Strings in the same order as the original list.

public static ArrayList<Integer> lengths(ArrayList<String> list) {
    // write your code here
}

public static void main(String[] args) {
    ArrayList<String> list = new ArrayList<String>();
    list.add("Hallo");
    list.add("Moi");
    list.add("Benvenuto!");
    list.add("badger badger badger badger");
    ArrayList<Integer> lengths = lengths(list);

    System.out.println("The lengths of the Strings: " + lengths);
}
    

Program output:


The lengths of the Strings: [5, 3, 10, 27]
    

The Greatest

Create the method greatest, which receives a list of numbers (ArrayList<Integer>) as a parameter and then returns the greatest number in the list as a return value.

public static int greatest(ArrayList<Integer> list) {
    // write your code here
}

public static void main(String[] args) {
    ArrayList<Integer> list = new ArrayList<Integer>();
    list.add(3);
    list.add(2);
    list.add(7);
    list.add(2);

    System.out.println("The greatest number is: " + greatest(list));
}
    

Program output:


The greatest number is: 7
    

Variance

Create the method variance, which receives a list of integers as a parameter and then returns the sample variance of that list. You can check how a sample variance is calculated in Wikipedia, under "Population variance and sample variance".

Note: the method should use the method average of exercise 64 to calculate the average of the parameters. The method should be called only once!

public static double variance(ArrayList<Integer> list) {
    // write your code here
}

public static void main(String[] args) {
    ArrayList<Integer> list = new ArrayList<Integer>();
    list.add(3);
    list.add(2);
    list.add(7);
    list.add(2);

    System.out.println("The variance is: " + variance(list));
}
    

Program output:


The variance is: 5.666667
    

(The average of the numbers is 3.5, so the sample variance is ((3 - 3.5)² + (2 - 3.5)² + (7 - 3.5)² + (2 - 3.5)²)/(4 - 1) ? 5,666667.)

Note while testing your program! Sample variance for a list that contains only one item is not defined! It causes a division by zero in the formula. Java considers the result of division by zero as a Not a Number (NaN).
Using truth values

A variable of type truth value (boolean) can only have two values: either true or false). Here is an example on how to use boolean variables:

int num1 = 1;
int num2 = 5;

boolean firstGreater = true;

if (num1 <= num2) {
    firstGreater = false;
}

if (firstGreater==true) {
    System.out.println("num1 is greater");
} else {
    System.out.println("num1 was not greater");
}

First, we assign the truth value variable firstGreater the value true. The first if sentence checks whether num1 is less or equal to num2. If it is, we change the value of firstGreater to false. The later if sentence selects which string to print based on the truth value.

As a matter of fact, using a truth value in a conditional sentence is easier than the description in the previous example. We can write the second if sentence as follows:

if (firstGreater) {  // means the same as firstGreater==true
    System.out.println("num1 was greater");
} else {
    System.out.println("num1 was not greater");
}

If we want to check if the boolean variable holds the value true, we do not need to write ==true, just writing the name of the variable is enough!

If we want to check if the boolean variable holds the value false, we can check that using the negation operation ! (exclamation mark):

if (!firstGreater) {  // means the same as firstGreater==false
    System.out.println("num1 was not greater");
} else {
    System.out.println("num1 was greater");
}

Methods that return a truth value

Truth values come in especially handy when we want to write methods that check for validity. Let us create a method that checks if the list it gets as a parameter includes only positive numbers (here 0 is considered positive). The method returns the information as a boolean (i.e. truth value).

public static boolean allPositive(ArrayList<Integer> numbers) {
    boolean noNegative = true;

    for (int number : numbers) {
        if (number < 0) {
            noNegative = false;
        }
    }

    // if one of the numbers on the list had a value that is below zero, noNegatives becomes false.

    return noNegative;
}

The method has a boolean helper variable called noNegative. First we assign the helper variable the value true. The method checks all numbers on the list one by one. If at least one number is less than 0, we assign the helper variable the value false. In the end the method returns the value of the helper variable. If no negative numbers were found, it has the value true, otherwise it has the value false.

The method is used as follows:

public static void main(String[] args) {

    ArrayList<Integer> numbers = new ArrayList<Integer>();
    numbers.add(3);
    numbers.add(1);
    numbers.add(-1);

    boolean result = allPositive(numbers);

    if (result) {  // means the same as result == true
        System.out.println("all numbers are positive");
    } else {
        System.out.println("there is at least one negative number");
    }
}

Usually it is not necessary to store the answer into a variable. We can write the method call directly as the condition:

ArrayList<Integer> numbers = new ArrayList<Integer>();
numbers.add(4);
numbers.add(7);
numbers.add(12);
numbers.add(9);

if (allPositive(numbers)) {
    System.out.println("all numbers are positive");
} else {
    System.out.println("there is at least one negative number");
}

The return command and ending a method

The execution of a method is stopped immediately when a command called return is executed. Using this information to our advantage, we write the allPositive method easier to understand.

public static boolean allPositive(ArrayList<Integer> numbers) {
    for (int number : numbers) {
        if (number < 0) {
            return false;
        }
    }

    // if the execution reached this far, no negative numbers were found
    // so we return true
    return true;
}

When we are going through the list of numbers and we find a negative number, we can exit the method by returning false. If there are no negative numbers on the list, we get to the end and therefore can return the value true. We now got rid of the helper variable inside the method!
Is the number more than once in the list?

Create the method moreThanOnce that gets a list of integers and an integer (i.e. number) as parameter. If the number appears on the list more than once the method returns true and otherwise false.

The program body is the following:

public static boolean moreThanOnce(ArrayList<Integer> list, int number) {
    // write your code here
}

public static void main(String[] args) {
    Scanner reader = new Scanner(System.in);

    ArrayList<Integer> list = new ArrayList<Integer>();
    list.add(3);
    list.add(2);
    list.add(7);
    list.add(2);

    System.out.println("Type a number: ");
    int number = Integer.parseInt(reader.nextLine());
    if (moreThanOnce(list, number)) {
        System.out.println(number + " appears more than once.");
    } else {
        System.out.println(number + " does not appear more than once.");
    }
}
    


Type a number: 2
2  appears more than once
    


Type a number: 3
3 does not appear more than once.
    

Palindrome

Create the method palindrome that checks if a string is a palindrome (reads the same forward and backward).

The method can use the method reverse (from assignment number 56. Reversing text) as a helper. The method type is boolean, so it returns either true (the string is a palindrome) or false (the string is not a palindrome).

public static boolean palindrome(String text) {
    // write your code here
}

public static void main(String[] args) {
    Scanner reader = new Scanner(System.in);

    System.out.println("Type a text: ");
    String text = reader.nextLine();
    if (palindrome(text)) {
       System.out.println("The text is a palindrome!");
    } else {
       System.out.println("The text is not a palindrome!");
    }
}
    

Example outputs:


Type a text: madam
The text is a palindrome!
    


Type a word: example
The text is not a palindrome!
    

-------------------------------------------------------------------------------------------------------------------------------

Methods and copying parameters

Let us focus on a couple of details concerning methods.

In section 15 was an example, in which we tried to change the value of a main program variable inside a method.

public static void main(String[] args) {
    int number = 1;
    addThree();
    System.out.println("Main program variable number holds the value: " + number);
}

public static void addThree() {
    number = number + 3;
}
  

This program of ours does not work. The reason is that the method cannot access the main program variable number.

This is because main program variables are not visible to methods. More generally: no method variable is visible to other methods. As the main program main is also a method, this constraint holds for the main program as well. The only way to give information to a method is through parameters.

Let us try to fix the above example by passing the main program variable number to the method as a parameter.

public static void main(String[] args) {
    int number = 1;
    addThree(number);
    System.out.println(number);  // prints 1, the value did not change
}

public static addThree(int number) {
    number = number + 3;
}
  

Still, the program does not function the way we want. The method parameters are different variables than the ones introduced in the main program. In the previous example, the method increments a variable with the same name as the main program variable. The parameter has the same name, but is not the same as the main program variable number.

When a parameter is given to a method, the value of the parameter is copied into a new variable and that new variable is the one the method uses. In the example above, the variable number that was given to the method addThree as a parameter, will be copied and then the copy is actually handed out for the method to use. The method uses a copy of the variable from the main program, not the original variable. The main program variable number stays unchanged.

We can imagine that the main program method main and the method addThree both work in their own parts of the computer memory. In the picture below, there is a "box" for the value of the variable number of the main method. When the method is called, a new "box" named number will be created and the main value of the method variable number will be copied into it. In this example, the number is 1. Both variables that are called number are separate, therefore when the method addThree changes the value of its own variable called number it does not affect the variable number in the main program.

The picture below will demonstrate what happens.

The method can still naturally pass information to the caller, which happens by using a return value (i.e. using a return command to return a variable with a value). We can get the previous example to work by changing the code a little bit:

public static void main(String[] args) {
    int number = 1;
    number = addThreeAndReturn(number);

    System.out.println(number);  // prints 4, because number has the method return value as its value
}

public static int addThreeAndReturn(int number) {
    number = number + 3;

    return number;
}
  

The method still uses the copy of the main program variable number. In the main program, we assign the variable number the method return value as a new value, so that we can get the change to take effect in the main program. Note that the name of the method variable plays no role here. The code works exactly the same regardless of the variable names. Here follows an example:

public static void main(String[] args) {
    int number = 1;
    number = addThreeAndReturn(number);

    System.out.println(number);
}

public static int addThreeAndReturn(int incremented) {
    incremented = incremented + 3;

    return incremented;
}
  

We have now found out that the parameters in methods are different variables than the variables introduced in the method call. Only the parameter value gets copied from the caller to the method.

Unfortunately this is not the whole story. If a method gets an ArrayList as a parameter, the method sees the original list and all the changes the method makes will take effect everywhere.

public static void removeFirst(ArrayList<Integer> list) {
    list.remove(0); // removes the number from index 0
}
  

public static void main(String[] args) {
    ArrayList<Integer> numbers = new ArrayList<Integer>();
    numbers.add(4);
    numbers.add(3);
    numbers.add(7);
    numbers.add(3);

    System.out.println(numbers); // prints [4,3,7,3]

    removeFirst(numbers);

    System.out.println(numbers); // prints [3,7,3]
}
  

Unlike a parameter of int type, a list will not be copied and therefore the method makes changes to the original list given as a parameter.

The picture below will clarify the example. ArrayList does not live in an imagined "box" like an int. The variable name in the example numbers is only a reference that refers to the place where the ArrayList is. One way to visualize this is that an ArrayList is connected with a wire. The name of the ArrayList is a "wire", and the list itself is located "at the other end of the wire". When we give the ArrayList to a method as a parameter, we actually give the method a wire. When the method uses its parameter, it finds the original list at the other end of this wire. Actually the main program and the method do have separate wires, but both wires have the same original list at the end of them and all the changes will be made directly to the original list. During and after this week we will find out that many things in Java are "connected with a wire".

Note that again the parameter name inside the method can be anything. It does not need to be the same as the name in the main program (or other method that calls it). In the example above, the method uses the name list but the method caller sees the same list with a different name: numbers.

Now, you probably start to wonder why does the value of the parameter get copied and the original variable stay intact when the parameter is of int type, but the original list is given to the method when the parameter is of ArrayList type? In Java only the values of primitive data types (which are int, double, char, boolean and a couple of others that we have not yet discussed) get copied to the method. When the method parameters are of other types only the references are copied to the method. A reference is like a "wire", therefore the method can access the list using it directly. The variables that are not of primitive data types are of reference data types and are "wired" just like the ArrayList in the previous example. The method is given the wire and the method can access the parameter directly.
Combining ArrayLists

Create the method public static void combine(ArrayList<Integer> first, ArrayList<Integer> second) that inserts the items in a list called second to a list called first. The order of the items can be anything and the same item can appear in the list more than once. An example on using the method:

ArrayList<Integer> list1 = new ArrayList<Integer>();
ArrayList<Integer> list2 = new ArrayList<Integer>();

list1.add(4);
list1.add(3);

list2.add(5);
list2.add(10);
list2.add(7);

combine(list1, list2);

System.out.println(list1); // prints [4, 3, 5, 10, 7]

System.out.println(list2); // prints [5, 10, 7]
      

We can use the method addAll provided by the ArrayList class to add one list in another list. The list gets the other list, whose items are to be added, as a parameter.
Smart combining

Create the method smartCombine that works like the previous combine method except that numbers can be on the list only once. This means that the method adds a new number to the list only if the list does not already contain that number. You might find the method contains from the ArrayList class useful. You can use that method to check if a number is in the list.
Instructions on code-writing and problem solving

Two of the leading software developers, Martin Fowler and Kent Beck have said in the book Refactoring: Improving the Design of Existing Code that:

    Fowler: "Any fool can write code that a computer can understand. Good programmers write code that humans can understand."
    Beck: "I'm not a great programmer, I'm just good a programmer with great habits."

[Update: previously both quotes were credited to Kent Beck. Our thanks go to Esko Luontola for pointing out this mistake]:

We are now taking the first steps towards becoming good programmers.
Well indented and "breathing" code

Let us take a look at a code that first adds numbers to a list and then prints the items fo the list. Then all instances of a certain number are removed from the list and the list gets printed.

First, we write the code badly and without indentations:


public static void main(String[] args) {
ArrayList<Integer> numbers = new ArrayList<Integer>();
numbers.add(4);
numbers.add(3);
numbers.add(7);
numbers.add(3);
System.out.println("The numbers in the beginning:");
for (int number : numbers) {
System.out.println(number);
}
while (numbers.contains(Integer.valueOf(3))) {
numbers.remove(Integer.valueOf(3));
}
System.out.println("The numbers after removal:");
for (int number : numbers) {
System.out.println(number);
}

Even though the unindented code works, it is unpleasant to read. Let us indent the code (you can get NetBeans to auto-indent your code by pressing Alt+Shift+F) and separate logical parts with line breaks:

public static void main(String[] args) {
    ArrayList<Integer> numbers = new ArrayList<Integer>();
    numbers.add(4);
    numbers.add(3);
    numbers.add(7);
    numbers.add(3);

    System.out.println("The numbers in the beginning:");

    // here we print numbers
    for (int number : numbers) {
        System.out.println(number);
    }

    // checks if the list contains the number 3
    while (numbers.contains(Integer.valueOf(3))) {
        numbers.remove(Integer.valueOf(3));  // if yes, it is removed
    }
    // we use a while structure to get all the threes removed!

    System.out.println("The numbers after removal:");

     // here we print numbers
    for (int number : numbers) {
        System.out.println(number);
    }
}

Now, the code starts to make sense. For example, the printing and the number removal are two logical parts, therefore they are separated with line breaks. The code is airy and reading the code is much more pleasant.

There are even comments in the code to help the reader understand what happens and where!
Getting rid of copy-paste with methods

What could be called the Original sin of a programmer is to create copy-paste code. This means using the same code in multiple places by copy-pasting it around the source code. In our example, the printing of the list is done twice. The code that handles the printing part should be separated as its own method. Then the printing method should be called from the main program:

public static void main(String[] args) {
    ArrayList<Integer> numbers = new ArrayList<Integer>();
    numbers.add(4);
    numbers.add(3);
    numbers.add(7);
    numbers.add(3);

    System.out.println("The numbers in the beginning:");

    // here we print numbers
    print(numbers);

    while (numbers.contains(Integer.valueOf(3))) {
        numbers.remove(Integer.valueOf(3));
    }

    System.out.println("The numbers after removal:");

    // here we print numbers
    print(numbers);
}

public static void print(ArrayList<Integer> numbers) {
    for (int number : numbers) {
        System.out.println( number );
    }
}

Slicing separate tasks into methods with descriptive names

Now, the code has become even more easy to read. A distinctively separate entity, the printing of the list is now a method that is easy to understand. By defining a new method the readability of the main program has improved. Pay attention to the descriptive name of the method: the name describes exactly what the method does. Next, we can remove the advising comments here we print numbers , because the name of the method speaks for itself.

There is still room for improvements in writing the program. The main program still looks a bit messy, since there is an "unaesthetic" code line that directly manipulates the list, in between the neat method calls. Let us turn that unaesthetic piece of code into a method:

public static void main(String[] args) {
    ArrayList<Integer> numbers = new ArrayList<Integer>();
    numbers.add(4);
    numbers.add(3);
    numbers.add(7);
    numbers.add(3);

    System.out.println("The numbers in the beginning:");
    print(numbers);

    remove(numbers, 3);

    System.out.println("The numbers after removal:");
    print(numbers);
}

public static void print(ArrayList<Integer> numbers) {
    for (int number : numbers) {
        System.out.println( number );
    }
}

public static void remove(ArrayList<Integer> numbers, int removed) {
    while (numbers.contains(Integer.valueOf(removed))) {
        numbers.remove(Integer.valueOf(removed));
    }
}

In the example above, we created a new descriptively named method out of a separate logical entity, i.e. removing all the instances of a certain number. The resulting main program is now very understandable - almost like natural language. Both methods are very simple and easy to understand as well.

Kent Beck might be proud of what we have accomplished! The code is easy to understand, easy to modify and does not include any copy-paste.
Object-oriented programming

Before we begin, here is a small introduction to object-oriented programming.

In procedural programming - which is the way of programming we have been studying so far - a program is divided in to smaller parts, methods. A method works as a separate part of a program and it can be called from anywhere in the program. When a method is called, execution of the program moves to the beginning of the called method. After the execution of the method is done, the program will continue from where the method was called.

In object oriented programming, just like in procedural programming, we attempt to divide a program into smaller parts. In object-oriented programming the small parts are objects. Each separate object has its own individual responsibility; an object contains a related group of information and functionality. Object-oriented programs consist of multiple objects which together define how the program works.
Object

We have already used many of the ready-made objects in Java. For example, ArrayLists are objects. Each separate list consists of information related to it; that is, the state of the object. Functionality is also contained in the ArrayList objects: the methods by which the state of the object can be altered. As an example, there are two ArrayList objects in the following piece of code, cities and countries :

public static void main(String[] args) {
    ArrayList<String> cities = new ArrayList<String>();
    ArrayList<String> countries = new ArrayList<String>();

    countries.add("Finland");
    countries.add("Germany");
    countries.add("Netherlands");

    cities.add("Berliini");
    cities.add("Nijmegen");
    cities.add("Turku");
    cities.add("Helsinki");

    System.out.println("number of countries " + countries.size() );
    System.out.println("number of cities " + cities.size() );
}

Both the countries object and the cities object live a life of their own. The state of each is not related to the state of the other. For example, the state of the countries object consists of the Strings "Finland", "Germany" and "Netherlands" that are in the list, probably also the information of how many countries are in the list.

When doing a method call related to an object (for example, countries.add("Finland");), the name of the object whose method is being called goes to the left side of the period sign (dot), and to the right side goes the name of the method itself. When asking how many Strings the countries list contains, we call countries.size(). We are calling the method size of the object countries. What the method returns depends on the state of the object in question, other objects do not affect the execution of the method in any way.

We have used the command new many times already. For example, creation of a list (ArrayList) and creation of a reader (Scanner) have been done using the command new. The reason is that both of these are classes from which the object is created. In Java, objects are always created with new, except in a few cases.

One of the cases where you do not always need to use new is in the construction of Strings. The familiar way to create a String is actually an abbreviated way of using new. A String can also be created with new just like any other object:

String text = "some text";       // abbreviated way of creating a String
String anotherText = new String("more text");

Cases in which ready-made parts of Java call new out of sight of the programmer also exist.
Class

It is clear that all objects are not similar to one another. For example, ArrayList objects differ drastically from String objects. All ArrayLists have the same methods add, contains, remove, size, ... and respectively all String objects have the same methods (substring, length, charAt, ...). Arraylist and String objects do not have the same methods because they are different types of objects.

The type of a certain group of objects is called a class. ArrayList is a class, as are String, Scanner, and so forth. Objects, on the other hand, are instances of classes.

Objects of the same class all have the same methods and a similar state. For example, the state of an ArrayList object consists of elements inserted to the list while the state of a String object consists of a string of characters.
A class and its objects

A class defines what kind of objects it has:

    what methods the objects have
    what the state of the objects are, or in other words, what kind of attributes the objects have

A class describes the "blueprint" of the objects that are made out of it (are instances of it).

Lets take an analogy from the world outside of computers: the blueprints of a house. The blueprints define how the building is to be built and in that way dictate the shape and size of it. The blueprints are the class, they define the general characteristics of the objects created out of that class:

Individual objects, the houses in our analogy, are made from that same blueprint. They are instances of the same class. The state of individual objects, the attributes, can vary (color of walls, building material of the roof, doors, windowsills, etc...). Here is one instance of a House object:

An object is always created from its class by calling the method - the constructor - that creates the object with the command new. For example, a new instance is created from the class Scanner by calling new Scanner(..):

Scanner reader = new Scanner(System.in);

Constructors take parameters the way any other method does.
Accounts

You are handed a ready-made class Account along with your exercise files. The object of the class Account represents a bank account that has a balance (meaning some amount of money). The accounts are used as follows:

Account bartosAccount = new Account("Barto's account",100.00);
Account bartosSwissAccount = new Account("Barto's account in Switzerland",1000000.00);

System.out.println("Initial state");
System.out.println(bartosAccount);
System.out.println(bartosSwissAccount);

bartosAccount.withdrawal(20);
System.out.println("Barto's account balance is now: "+bartosAccount.balance());
bartosSwissAccount.deposit(200);
System.out.println("Barto's Swiss account balance is now: "+bartosSwissAccount.balance());

System.out.println("Final state");
System.out.println(bartosAccount);
System.out.println(bartosSwissAccount);
    

Your first account

Note: there is a different exercise template for each of the sub-exercises. For this exercise use the template 072.1

Create a program that creates an account with the balance of 100.0, deposits 20.0 and prints the account. Note! do all the steps described in the exercise exactly in the described order!
Your first money transfer

Note: there is a different exercise template for each of the sub-exercises. For this exercise use the template 072.2

Create a program that:

    Creates an account named "Matt's account" with the balance of 1000
    Creates an account named "My account" with the balance of 0
    Withdraws 100.0 from Matt's account
    Deposits 100.0 to My account
    Prints both accounts

Money transfers

Note: there is a different exercise template for each of the sub-exercises. For this exercise use the template 072.3

In the above program, you made a money transfer from one person to another. Let us next create a method that does the same!

Create the method public static void transfer(Account from, Account to, double howMuch) in the given program body. The method transfers money from one account to another. You do not need to check that the from account has enough balance.

After completing the above, make sure that your main method does the following:

    Creates an account "A" with the balance of 100.0
    Creates an account "B" with the balance of 0.0
    Creates an account "C" with the balance of 0.0
    Transfers 50.0 from account A to account B
    Transfers 25.0 from account B to account C

Defining your own class - object variables

A class is defined to serve some meaningful whole. Often a "meaningful whole" represents something from the real world. If a computer program needs to handle personal data it could be sensible to define a separate class Person which then holds methods and attributes related to an individual.

Let us go ahead and assume that we have a project frame with an empty main program:

public class Main {

    public static void main(String[] args) {
    }

}

We will create a new class in our project. In NetBeans, this can be done in projects on the left, from the right click menu select new, java class. We will name the class in the dialog that pops up.

Just as with variables and methods, the name of the class should always be as descriptive as possible. Sometimes as a project progresses a class might transform into something different in order meet the programmer's needs. In situations like this, it is possible to rename your class with ease (see the NetBeans guide).

Let us create a class named Person. The class will exist in its own Person.java file. Since the main program is in its own file the program now consists of two files in total. At first the class will be empty:

public class Person {

}

The class has to define what methods and attributes the objects created from the class will have. Let us decide that each person has a name and an age. It feels natural to represent the name as a String and the age as an integer. Let us add this to our schematics:

public class Person {
    private String name;
    private int age;
}

Above, we defined that all instances created from the Person class have a name and an age. Defining attributes is done in a quite similar fashion as with normal variables. In this case though, there is the keyword private in front. This keyword means that name and age will not show outside of the object, but are instead hidden within it. Hiding things within an object is called encapsulation.

Variables defined within a class are called object variables, object fields or object attributes. A beloved child has many names.

So, we have defined the schematics -- the class -- for the person object. All person objects have the variables name and age. The 'state' of the objects is determined by the values that have been set to its variables.
Defining your own class - constructor, or "formatting the state"

When an object is created its starting state is defined at the same time. Self-defined objects are created for the most part in the same way as ready-made objects (ArrayList objects for example) are created. Objects are created with the new command. When creating an object it would be handy to be able to set the values of some of the variables of that object.

    public static void main(String[] args) {
        Person bob = new Person("Bob");
        // ...
    }

This can be achieved by defining the method that creates the object, the constructor. The constructor for the Person class that creates a new Person object has been defined in the following example. In the constructor, the person that is being created gets 0 as her age and her name is received from the parameter of the constructor.

public class Person {
    private String name;
    private int age;

    public Person(String initialName) {
        this.age = 0;
        this.name = initialName;
    }
}

The constructor always has the same name as the class. In the code above, the class is Person and the constructor is public Person(String initialName). The value the constructor receives as a parameter is in parentheses after the name of the constructor. You can imagine the constructor as a method that Java runs when an object is created with the command new Person("Bob"); Whenever an object is created from a class, the constructor of that class is called.

A few notes: within the constructor there is a command this.age = 0. Through it, we set a value for this particular object; we define the internal variable age of "this" object. Another command we use is this.name = initialName;. Again, we give the internal variable called name the String that is defined in the constructor. The variables age and name are automatically visible in the constructor and elsewhere in the object. They are referred to with the this prefix. Due to the private modifier, the variables cannot be seen from outside the object.

One more thing: if the programmer does not create a constructor for her class, Java will automatically create a default constructor for it. A default constructor is a constructor that does nothing. So, if you for some reason do not need a constructor you do not need to write one.
Class definition - methods

We already know how to create and initialize objects. However, objects are useless if they cannot do anything. Therefore, objects should have methods. Let us add to the Person class a method that prints the object on the screen:

public class Person {
    private String name;
    private int age;

    public Person(String nameAtStart) {
        this.age = 0;
        this.name = nameAtStart;
    }

    public void printPerson() {
        System.out.println(this.name + ", age " + this.age + " years");
    }
}

As seen above, the method is written within the class. The method name is prefixed with public void since it is assumed that users of the object should be capable of using the method and the method should not return anything. With objects the keyword static is not used in method definitions. Next week, we will clarify the reason behind that.

Inside the method printPerson, there is a single line of code that uses the object variables name and age. The prefix this is used to emphasize that we are referring to the name and age of this object. All the object variables are visible from all the methods of the object.

Let us create three persons and ask them to print themselves:

public class Main {

    public static void main(String[] args) {
        Person pekka = new Person("Pekka");
        Person brian = new Person("Brian");
        Person martin = new Person("Martin");

        pekka.printPerson();
        brian.printPerson();
        martin.printPerson();
    }
}

The output is:

Pekka, age 0 years
Brian, age 0 years
Martin, age 0 years

Product

Create a class Product that represents a product sold in a webshop. A product has a price, amount and name.

A new class can be created as follows: Point at the project 073.Product in the projects tab and click the right mouse button. Then select new and java class. When a dialog opens, give the class the name Product.

The class should have:

    A constructor public Product(String nameAtStart, double priceAtStart, int amountAtStart)
    A method public void printProduct() that prints a product in the following form:

    Banana, price 1.1, amount 13
          

More methods

Let us create a method that can be used to increase the age of a person by one:

public class Person {
    // ...

    public void becomeOlder() {
        this.age++;;    // same as this.age = this.age + 1;
    }
}

As expected, the method is written inside the class Person. The method increases the value of object variable age by one.

Let us call the method and see what happens:

public class Main {

    public static void main(String[] args) {
        Person pekka = new Person("Pekka");
        Person andrew = new Person("Andrew");

        pekka.printPerson();
        andrew.printPerson();

        System.out.println("");

        pekka.becomeOlder();
        pekka.becomeOlder();

        pekka.printPerson();
        andrew.printPerson();
    }
}

Output:

Pekka, age 0 years
Andrew, age 0 years

Pekka, age 2 years
Andrew, age 0 years

When born, both objects have age 0 due to the line this.age = 0; in the constructor. The method becomeOlder of object pekka is called twice. As the output shows, this causes the age of pekka to increase by two. It should be noted that when the method becomeOlder is called in the object pekka, the other object andrew is not touched at all and he remains at age 0. The state of an object is independent of the other objects!

Also, the object methods can return a value to the caller of the method. Let us define a method that can be used to ask for the age of a person:

public class Person {
    // ...

    public int getAge() {
        return this.age;
    }
}

Now the void in the method definition is replaced with int since the value the method returns has the type integer. The following example demonstrates, how the value returned by a method can be used:

public class Main {

    public static void main(String[] args) {
        Person pekka = new Person("Pekka");
        Person andrew = new Person("Andrew");

        pekka.becomeOlder();
        pekka.becomeOlder();

        andrew.becomeOlder();

        System.out.println( "Age of Pekka: "+pekka.getAge() );
        System.out.println( "Age of Andrew: "+andrew.getAge() );

        int total = pekka.getAge() + andrew.getAge();

        System.out.println( "Pekka and Andrew total of "+total+ " years old" );
    }
}

Output:

Age of Pekka: 2
Age of Andrew: 1

Pekka and Andrew total of 3 years old

Multiplier

Implement the class Multiplier that has:

    a constructor public Multiplier(int number).
    a method public int multiply(int otherNumber) that returns otherNumber multiplied by number (i.e., the constructor parameter).

Example of usage:

Multiplier threeMultiplier = new Multiplier(3);
System.out.println("threeMultiplier.multiply(2): " + threeMultiplier.multiply(2));

Multiplier fourMultiplier = new Multiplier(4);
System.out.println("fourMultiplier.multiply(2): " + fourMultiplier.multiply(2));

System.out.println("threeMultiplier.multiply(1): " + threeMultiplier.multiply(1));
System.out.println("fourMultiplier.multiply(1): " + fourMultiplier.multiply(1));
    

Output

threeMultiplier.multiply(2): 6
fourMultiplier.multiply(2): 8
threeMultiplier.multiply(1): 3
fourMultiplier.multiply(1): 4
    

Decreasing counter

The starting point of this exercise is a partially implemented class DecreasingCounter:

public class DecreasingCounter {
    private int value;   // object variable that remembers the value of the counter

    public DecreasingCounter(int valueAtStart) {
        this.value = valueAtStart;
    }

    public void printValue() {
        System.out.println("value: " + this.value);
    }

    public void decrease() {
        // write here the code that decrements the value of counter by one
    }

    // and here the rest of the methods
}
    

The counter can be used as follows:

public class Main {
    public static void main(String[] args) {
        DecreasingCounter counter = new DecreasingCounter(10);

        counter.printValue();

        counter.decrease();
        counter.printValue();

        counter.decrease();
        counter.printValue();
    }
}
    

Output should be:

value: 10
value: 9
value: 8
    

The constructor of DecreasingCounter receives as parameter the initial value of the counter. In the example, the constructor parameter is 10, which is then set to the object variable this.value. The value of the counter can be printed with the method printValue(). The method decrease() should decrease the value of the counter by one.
Implementing method decrease()

Implement the method decrease() so that when called, the object variable this.value is decreased by one. When this is done, your program should work as the example above.
Value remains positive

Change your implementation of the method decrease() so that the value of the counter will not drop below zero. If the method is called when the value is zero, nothing should happen:

public class Main {
    public static void main(String[] args) {
        DecreasingCounter counter = new DecreasingCounter(2);

        counter.printValue();

        counter.decrease();
        counter.printValue();

        counter.decrease();
        counter.printValue();

        counter.decrease();
        counter.printValue();
    }
}
    

Output should be:

value: 2
value: 1
value: 0
value: 0
    

Counter reset

Implement the method public void reset() that sets the value of the counter to zero. Example of usage:

public class Main {
    public static void main(String[] args) {
        DecreasingCounter counter = new DecreasingCounter(100);

        counter.printValue();

        counter.reset();
        counter.printValue();

        counter.decrease();
        counter.printValue();
    }
}
    

Output:

value: 100
value: 0
value: 0
    

Back to initial value

Implement the method public void setInitial(), which returns the counter to its initial value:

public class Main {
    public static void main(String[] args) {
        DecreasingCounter counter = new DecreasingCounter(100);

        counter.printValue();

        counter.decrease();
        counter.printValue();

        counter.decrease();
        counter.printValue();

        counter.reset();
        counter.printValue();

        counter.setInitial();
        counter.printValue();
    }
}
    

Output:

value: 100
value: 99
value: 98
value: 0
value: 100
    

Hint: add to the class a new object variable that remembers the initial value of the counter
Menu

In this assignment, we will implement a class Menu that holds information about meals that are available in a cafeteria.

Our starting point is the following class skeleton:

import java.util.ArrayList;

public class Menu {

    private ArrayList<String> meals;

    public Menu() {
        this.meals = new ArrayList<String>();
    }

    // Implement the methods here
}
    

Menu objects store the information of meals using an object variable of type ArrayList<String>
Adding a meal to menu

Implement the method public void addMeal(String meal) that adds a new meal to the list this.meals of a Menu object. If the meal is already in the list, it should not be added.
Printing the menu

Implement the method public void printMeals() that prints the meals in a menu. As an example, the output after three additions could be:

Hamburger
Fish'n'Chips
Sauerkraut
    

Clearing a menu

Implement the method public void clearMenu() that clears a menu. After calling this method, the menu should be empty. Class ArrayList has a method that is useful here. Within your method body write meals. and see how NetBeans helps you by showing the available methods.
The Person class grows

Let us get back to work on the Person class. The current version of the class looks like this:

public class Person {
    private String name;
    private int age;

    public Person(String initialName) {
        this.age = 0;
        this.name = initialName;
    }

    public void printPerson() {
        System.out.println(this.name + ", age " + this.age + " years");
    }

    public void becomeOlder() {
        this.age = this.age + 1;
    }
}

Let us create a method for person that can figure out if a person is an adult. The method returns a boolean -- either true or false:

public class Person {
    // ...

    public boolean isAdult(){
        if ( this.age < 18 ) {
            return false;
        }

        return true;
    }

   /*
      note that the method could also be written like this:
  
      public boolean isAdult(){
        return this.age >= 18;
      }
   */
}

Let us test it:

    public static void main(String[] args) {
        Person bob = new Person("Bob");
        Person andy = new Person("Andy");

        int i = 0;
        while ( i < 30 ) {
            bob.becomeOlder();
            i++;
        }

        andy.becomeOlder();

        System.out.println("");

        if ( andy.isAdult() ) {
            System.out.print("adult: ");
            andy.printPerson();
        } else {
            System.out.print("minor: ");
            andy.printPerson();
        }

        if ( bob.isAdult() ) {
            System.out.print("adult: ");
            bob.printPerson();
        } else {
            System.out.print("minor: ");
            bob.printPerson();
        }
    }

minor: Andy, age 1 years
adult: bob, age 30 years

Let us tune up the solution a little further. Now, a person can only be printed in a manner where in addition to the name, the age also gets printed. In some cases, we might only want to print the name of the object. Let us tailor a method for this purpose:

public class Person {
    // ...

    public String getName() {
        return this.name;
    }
}

The method getName returns the object variable name to its caller. The name of the method might seem a little odd (or not). In Java, it is considered the 'correct' way to name an object-variable-returning method in this manner; as getVariableName. Methods like these are often called 'getters'.

Let us edit the main program to use the new 'getter':

    public static void main(String[] args) {
        Person bob = new Person("bob");
        Person andy = new Person("andy");

        int i = 0;
        while ( i < 30 ) {
            bob.becomeOlder();
            i++;
        }

        andy.becomeOlder();

        System.out.println("");

        if ( andy.isAdult() ) {
            System.out.println( andy.getName() + " is an adult" );
        } else {
            System.out.println( andy.getName() + " is a minor" );
        }

        if ( bob.isAdult() ) {
            System.out.println( bob.getName() + " is an adult" );
        } else {
            System.out.println( bob.getName() + " is a minor" );
        }
    }

The print is starting to look pretty clean:

andy is a minor
bob is an adult

toString

We have been guilty of bad programming style; we have created a method that prints an object, printPerson. The recommended way of doing this is by defining a method that returns a "character string representation" of the object. In Java, a method returning a String representation is called toString. Let us define this method for person:

public class Person {
    // ...

    public String toString() {
        return this.name + ", age " + this.age + " years";
    }
}

The method toString works just like printPerson, but instead of printing it the method returns the string representation. The call to the method can be used for printing it if necessary.

The method is used in a slightly surprising way:

    public static void main(String[] args) {
        Person bob = new Person("Bob");
        Person andy = new Person("Andy");

        int i = 0;
        while ( i < 30 ) {
            bob.becomeOlder();
            i++;
        }

        andy.becomeOlder();

        System.out.println( andy ); // same as System.out.println( andy.toString() ); 
        System.out.println( bob ); // same as System.out.println( bob.toString() ); 
    }

The principle is that the System.out.println method requests the string representation of an object and then prints it. The returned string representation of the toString method does not have to be written, as Java adds it automatically. When the programmer writes:

        System.out.println( andy );

Java completes the call during runtime to the format:

        System.out.println( andy.toString() );

What happens is that the object is asked for its string representation. The string representation the object is returned and is printed normally with the System.out.println command.

We can get rid of the obsolete printObject method.
Lyyra-card

The University of Helsinki students use a so-called Lyyra cards to pay for their meals in student cafeterias. In this assignment, we implement the class LyyraCard that simulates the Lyyra card.
Class skeleton

Start by adding the class LyyraCard to your project.

Then implement the LyyraCard constructor that gets the starting balance of the card as parameter. The card saves the balance in the object variable balance. Implement also the toString method that returns a string of the form "The card has X euros".

The skeleton of class LyyraCard looks like this:

public class LyyraCard {
    private double balance;

    public LyyraCard(double balanceAtStart) {
        // write code here
    }

    public String toString() {
        // write code here
    }
}
    

The following main program can be used to test the program:

public class Main {
    public static void main(String[] args) {
        LyyraCard card = new LyyraCard(50);
        System.out.println(card);
    }
}
    

The output should be:

The card has 50.0 euros
    

Paying with card

Implement the following methods to LyyraCard:

public void payEconomical() {
    // write code here
}

public void payGourmet() {
    // write code here
}
    

Method payEconomical should decrease the balance by 2.50 euros and method payGourmet by 4.00 euros.

The following main program can be used to test the program:

public class Main {
    public static void main(String[] args) {
        LyyraCard card = new LyyraCard(50);
        System.out.println(card);

        card.payEconomical();
        System.out.println(card);

        card.payGourmet();
        card.payEconomical();
        System.out.println(card);
    }
}
    

The output should be:

The card has 50.0 euros
The card has 47.5 euros
The card has 41.0 euros
    

Balance nonnegative

Change methods payEconomical and payGourmet so that if there is not enought money, the balance does not change.

The following main program can be used to test the program:

public class Main {
    public static void main(String[] args) {
        LyyraCard card = new LyyraCard(5);
        System.out.println(card);

        card.payGourmet();
        System.out.println(card);

        card.payGourmet();
        System.out.println(card);
    }
}
    

The output should be:

The card has 5.0 euros
The card has 1.0 euros
The card has 1.0 euros
    

Above, the second call payGourmet does not alter the balance since there is not enough money on the card for a gourmet lunch.
Loading money to card

Add the LyyraCard the following method:

public void loadMoney(double amount) {
    // write code here
}
    

The method should increase the balance of the card by the given amount. However, the maximum balance on a card is 150 euros. In case the balance after loading money would be more than that, it should be truncated to 150 euros.

The following main program can be used to test the program:

public class Main {
    public static void main(String[] args) {
        LyyraCard card = new LyyraCard(10);
        System.out.println(card);

        card.loadMoney(15);
        System.out.println(card);

        card.loadMoney(10);
        System.out.println(card);

        card.loadMoney(200);
        System.out.println(card);
    }
}
    

The output should be:

The card has 10.0 euros
The card has 25.0 euros
The card has 35.0 euros
The card has 150.0 euros
    

Loading a negative amount

Change the method loadMoney so that the balance of the card does not change if the amount to load is negative.

The following main program can be used to test the program:

public class Main {
    public static void main(String[] args) {
        LyyraCard card = new LyyraCard(10);
        System.out.println("Pekka: " + card);
        card.loadMoney(-15);
        System.out.println("Pekka: " + card);
    }
}
    

The output should be:

Pekka: The card has 10.0 euros
Pekka: The card has 10.0 euros
    

Multiple cards

Write a main method that does the following:

    Creates a LyyraCard for Pekka with initial balance of 20 euros
    Creates a LyyraCard for Brian with initial balance of 30 euros
    Pekka buys gourmet lunch
    Brian buys economical lunch
    cards are printed (both on their own row, starting with the name of the card owner)
    Pekka loads 20 euros
    Brian buys gourmet lunch
    cards are printed (both on their own row, starting with the name of the card owner)
    Pekka buys economical lunch
    Pekka buys economical lunch
    Brian loads 50 euros
    cards are printed (both on their own row, starting with the name of the card owner)

The main skeleton is as follows:

public class Main {
    public static void main(String[] args) {
        LyyraCard cardPekka = new LyyraCard(20);
        LyyraCard cardBrian = new LyyraCard(30);

        // write code here
    }
}
    

The output should be:

Pekka: The card has 16.0 euros
Brian: The card has 27.5 euros
Pekka: The card has 36.0 euros
Brian: The card has 23.5 euros
Pekka: The card has 31.0 euros
Brian: The card has 73.5 euros
    

More methods

Let us continue with the class Person. We would be interested in knowing the body mass index of a person. To calculate the index, we need to know the height and weight of the person. We add for both height and weight object variables and methods that can be used to assign the variables a value. When this is in place, we add a method that calculates the body mass index.

Here is the class Person after the changes (only the parts affected by the change are shown):

public class Person {
    private String name;
    private int age;
    private int weight;
    private int height;

    public Person(String initialName) {
        this.age = 0;
        this.name = initialName;
        this.weight = 0;
        this.height = 0;
    }

    public void setHeight(int newHeight) {
        this.height = newHeight;
    }

    public void setWeight(int newWeight) {
        this.weight = newWeight;
    }

    public double bodyMassIndex(){
        double heightDividedByHundred = this.height / 100.0;
        return this.weight / ( heightDividedByHundred * heightDividedByHundred );
    }

    // ...
}

We added object variables height and weight, and methods setHeight and setWeight that can be used to give values to the variables. In naming the methods, we follow the Java convention to call a method that just sets a new value to a variable setVariableName. This type of methods are usually called setter methods.

The new methods in use:

public static void main(String[] args) {
    Person matti = new Person("Matti");
    Person john = new Person("John");

    matti.setHeight(180);
    matti.setWeight(86);

    john.setHeight(175);
    john.setWeight(64);

    System.out.println(matti.getName() + ", body mass index: " + matti.bodyMassIndex());
    System.out.println(john.getName() + ", body mass index: " + john.bodyMassIndex());
}

The output:

Matti, body mass index: on 26.54320987654321
John, body mass index: on 20.897959183673468

Object variable and parameter with identical name

Above, the method setHeight assigns the object variable height the value of the parameter newHeight:

public void setHeight(int newHeight) {
    this.height = newHeight;
}

The parameter could also be named identically with the object variable:

public void setHeight(int height) {
    this.height = height;
}

Now, the name height means the parameter height and the identically named object variable is referred to as this.height. The following would not work since the object variable height is not at all referred to in the code:

public void setHeight(int height) {
    // DOES NOT WORK!
    height = height;
    // this just assigns the value of the parameter to the parameter itself
}

Contolling the number of decimals when printing a float

The number of decimals in the last output was far too high, two decimals would be enough. One technique to control how a float number is printed is to use the command String.format.

If value is a float number, the command String.value( "%.2f", value ) returns a string where the value is rounded to contain 2 decimals. The number between dot and f defines the amount of decimals shown.

After changing the code, we have the following:

System.out.println(matti.getName() + ", body mass index: " + String.format( "%.2f", matti.bodyMassIndex()));
System.out.println(john.getName() + ", body mass index: " + String.format( "%.2f", john.bodyMassIndex()));

The output is:

Matti,  body mass index: 26,54
John,  body mass index: 20,90

The method String.format is not the most flexible way provided by Java for formatting float values, but it is simple to use and suits our purposes here well.
Clock using a counter

We start by implementing a class BoundedCounter and then use counter objects to implement a clock.
BoundedCounter

Implement class BoundedCounter with the following functionality:

    A counter has an object variable that remembers the value of the counter. The value is within the range 0..upperBound
    In the beginning the value is 0.
    The upper bound of the value is defined by the constructor parameter.
    The method next increments the value of the counter. If the value would be more that the upper limit, it wraps around and becomes zero.
    The method toString returns a string representation of the counter value.

The skeleton of the class is as follows:

public class BoundedCounter {
    private int value;
    private int upperLimit;

    public BoundedCounter(int upperLimit) {
        // write code here
    }

    public void next() {
        // write code here
    }

    public String toString() {
        // write code here
    }
}
    

Note: you cannot return an integer value directly from the method toString since the method should return a string. Integer variable value can be turned into a string by prefixing it with an empty string: "" + value.

A main program that uses the counter:

public class Main {
    public static void main(String[] args) {
        BoundedCounter counter = new BoundedCounter(4);
        System.out.println("Value at start: " + counter );

        int i = 0;
        while ( i < 10) {
            counter.next();
            System.out.println("Value: " + counter );
            i++;
        }
    }
}
    

In the constructor, an upper limit of 4 is given to the new counter object. Now, the value of the counter should be within the range 0...4. Note how the method next increases the value until it hits the upper limit and becomes zero again:

Value at start: 0
Value: 1
Value: 2
Value: 3
Value: 4
Value: 0
Value: 1
Value: 2
Value: 3
Value: 4
Value: 0
    

Printing the initial zero

Imrove toString so that if the value of the counter is less than 10, it prefixes the value with 0. If the value of the counter is e.g. 3, toString should produce "03". If the value is at least 10, e.g. 12, the returned string would be "12".

A main program that demonstrates the desired functionality of the improved toString.

public class Main {
    public static void main(String[] args) {
        BoundedCounter counter = new BoundedCounter(14);
        System.out.println("Value at start: " + counter );

        int i = 0;
        while ( i < 16){
            counter.next();
            System.out.println("value: " + counter );
            i++;
        }
    }
}
    

value at start: 00
value: 01
value: 02
value: 03
value: 04
value: 05
value: 06
value: 07
value: 08
value: 09
value: 10
value: 11
value: 12
value: 13
value: 14
value: 00
value: 01
    

The first version of the clock

With two counter objects it possible for us to build a simple clock. Hours can be represented by a counter with upper bound 23 and minutes by a counter with upper bound 59. As we all know, when minutes wrap around from 59 to 0, hours advance by one.

First you should implement the method getValue for the counters in the class:

public int getValue() {
    // write here code that returns the value
}
    

Then implement the clock in your main method in the following style:

public class Main {
    public static void main(String[] args) {
        BoundedCounter minutes = new BoundedCounter(59);
        BoundedCounter hours = new BoundedCounter(23);

        int i = 0;
        while ( i < 121 ) {
            System.out.println( hours + ":" + minutes);   // the current time printed
            // advance minutes
            // if minutes become zero, advance hours
            i++;
        }
    }
}
    

The output should be:

00:00
00:01
...
00:59
01:00
01:01
01:02
...
01:59
02:00
    

The second version of the clock

Firstly implement the method setValue to the class BoundedCounter. The method should set the value of the parameter to the counter unless the parameter is less than zero or larger than the upper bound. In those cases, the method does not have any effect.

Then add a seconds counter to your clock. The clock should now be as follows:

public class Main {
    public static void main(String[] args)  {
        Scanner reader = new Scanner(System.in);
        BoundedCounter seconds = new BoundedCounter(59);
        BoundedCounter minutes = new BoundedCounter(59);
        BoundedCounter hours = new BoundedCounter(23);

        System.out.print("seconds: ");
        int s = // read the initial value of seconds from the user
        System.out.print("minutes: ");
        int m = // read the initial value of minutes from the user
        System.out.print("hours: ");
        int h = // read the initial value of hours from the user

        seconds.setValue(s);
        minutes.setValue(m);
        hours.setValue(h);

        int i = 0;
        while ( i < 121 ) {
            // like in previous but seconds taken into account

            i++;
        }

    }
}
    

Ensure that all works as expected when starting e.g. with time 23:59:50.

The output should be:

seconds: 50
minutes: 59
hours: 23
23:59:50
23:59:51
23:59:52
...
    

Bonus: eternal clock (exercise not assessed with TMC!)

Before you start, submit the exercise for assesment.

Change your main as follows:

public class Main {
    public static void main(String[] args) throws Exception {
        BoundedCounter seconds = new BoundedCounter(59);
        BoundedCounter minutes = new BoundedCounter(59);
        BoundedCounter hours = new BoundedCounter(23);

        seconds.setValue(50);
        minutes.setValue(59);
        hours.setValue(23);

        while ( true ) {
            System.out.println( hours + ":" + minutes + ":" + seconds );
            Thread.sleep(1000);
            // put here the logic to advance your clock by one second
        }
    }
}
    

Now, the clock goes on forever and the value is updated as it should be, once in a second. The clock estimates the duration of a second with the command Thread.sleep(1000); The parameter in the command is the time to sleep in milliseconds. In order to use the sleep command, you should do an addition to the definition of main: public static void main(String[] args) throws Exception {

You can end the eternal clock by pressing the red box in the NetBeans console (i.e. the area in NB where the output of programs gets printed).

Important notes regarding the use of objects. You should definately read these.

Object-oriented programming is mostly about turning concepts into their own entities, or in other words forming abstractions. One might think that it is pointless to create an object that only holds one number in it, and that the same could be achieved with simple int variables. This is not the case. If a clock consists of just 3 int variables that are then increased, the program loses some human readability. It becomes more difficult to "see" what the program is about. Earlier in the material we mentioned the advice of the renown programmer Kent Beck: "Any fool can write code that a computer can understand. Good programmers write code that humans can understand", since the hand of a clock is its own clearly definable concept, it is a good idea to create it an own class - BoundedCounter - for the sake of human readability.

Turning a concept into a class of its own is a good idea for a lot of reasons. Firstly, some details (i.e. when the counter makes a full round) can be hidden inside the class (abstracted). Instead of writing an if-clause and an assignment operation, it is enough that the user of the counter calls the descriptively named method next(). In addition to clocks, the created counter might be good for being used as a building block for other projects too, so a class made from a clear concept can be very versatile. Another huge advantage we gain by writing code this way, is that when the details of the mechanics are hidden, they can be changed if need be.

We established that a clock contains three hands, it consists of three concepts. Actually the clock itself is a concept too and next week we will make the class Clock. Then, we can create distinct Clock objects. Clock will be an object which functionality is based on "simpler" objects, the hands. This is the grand idea of object-oriented programming: a program is built out of small, clearly defined co-operating objects.

Now, we will take some careful first steps in the object world. Towards the end of the course, objects will start to come to you naturally and the idea of programs being built out of small, well defined, co-operating pieces - which at this point might feel incomprehensible - will become something you will take for granted.
Calling other methods within an object

Objects can also call its own methods. Let us assume we would like to include body mass index in the string representation of the person objects. Instead of calculating the body mass index in the toString method, a better idea is to call the method bodyMassIndex from the toString method:

public String toString() {
    return this.name + ", age " + this.age + " years, my body mass index is " + this.bodyMassIndex();
}

As can be seen, an object can call its own method by prefixing the method name with this and dot. The this is not necessary, so also the following works:

public String toString() {
    return this.name + ", age " + this.age + " years, my body mass index is " + bodyMassIndex();
}

Now it is time to continue practising programming.
NumberStatistics
Amount of numbers

Implement class NumberStatistics with the following methods:

    addNumber adds a new number to the statistics
    amountOfNumbers tells us how many numbers have been added to the statistics

Note that the class should not store the added numbers. At this stage, it is enough to remember how many added numbers there are, i.e. how many times the method addNumber has been called.

The class skeleton:

public class NumberStatistics {
    private int amountOfNumbers;

    public NumberStatistics() {
        // initialize here the object variable amountOfNumbers
    }

    public void addNumber(int number) {
        // code here
    }

    public int amountOfNumbers() {
        // code here
    }
}
    

A usage example:

public class Main {
   public static void main(String[] args) {
      NumberStatistics stats = new NumberStatistics();
      stats.addNumber(3);
      stats.addNumber(5);
      stats.addNumber(1);
      stats.addNumber(2);
      System.out.println("Amount: " + stats.amountOfNumbers());
    }
}
    

The output should be:

Amount: 4
    

sum and average

Add the following methods to the class:

    sum returns the sum of the added numbers (if no numbers added, the sum is 0)
    average returns the average of the added numbers (if no numbers added, the average is 0)

The class skeleton now:

public class NumberStatistics {
    private int amountOfNumbers;
    private int sum;

    public NumberStatistics() {
        // initialize here the object variable amountOfNumbers
    }

    public void addNumber(int number) {
        // code here
    }

    public int amountOfNumbers() {
        // code here
    }

    public int sum() {
        // code here
    }

    public double average() {
        // code here
    }
}
    

A usage example:

public class Main {
    public static void main(String[] args) {
        NumberStatistics stats = new NumberStatistics();
        stats.addNumber(3);
        stats.addNumber(5);
        stats.addNumber(1);
        stats.addNumber(2);
        System.out.println("Amount: " + stats.amountOfNumbers());
        System.out.println("sum: " + stats.sum());
        System.out.println("average: " + stats.average());
    }
}
    

The output should be:

Amount: 4
sum: 11
average: 2.75
    

Asking for numbers from the user

Create a program that asks the user to input numbers of type integer. When the user gives -1, the program stops and prints the sum of the given numbers (excluding the -1).

Note: you should not make any changes to class NumberStatistics!

The program should use a NumberStatistics object to calculate the sum.

Type numbers:
4
2
5
4
-1
sum: 15
    

Many sums

Change your program so that it also calculates the sum of even and odd numbers in the user input (again -1 excluded).

NOTE: define in your program three NumberStatistics objects. The first is used to track the sum of all the numbers. The second takes care of even numbers and the third the odd numbers. Remember also that you should not make any changes to class NumberStatistics!

The tests does not work if you do not create the objects in the order mentioned above!!

The program should work as follows:

Type numbers:
4
2
5
2
-1
sum: 13
sum of even: 8
sum of odd: 5
    

Randomness

When programming, you may occasionally need to simulate random events. Situations such as the unpredictability of weather, or surprising moves on the AI's part in a computer game can often be simulated with random number generators, running on a computer. In Java, there is a ready-made class Random, which you can use in the following way:

import java.util.Random;

public class Randomizing {
    public static void main(String[] args) {
        Random randomizer = new Random(); // creates a random number generator
        int i = 0;

        while (i < 10) {
            // Generates and prints out a new random number on each round of the loop
            System.out.println(randomizer.nextInt(10));
            i++;
        }
    }
}

In the code above, you first create an instance of the class Random with the keyword new -- exactly as when creating objects implementing other classes. An object of type Random has the method nextInt that can be given an integer value as parameter. The method returns a random integer within the range 0..(the integer given as parameter- 1).

The printout of this program could be as follows:

2
2
4
3
4
5
6
0
7
8

We will need floating point numbers, for example when dealing with probability calculations. In computing, probabilities are usually calculated with numbers within the range [0..1]. An object of the class Random can return random floating point numbers with the method nextDouble. Let us consider the following probabilities of weather conditions:

    Sleet with the probability 0.1 (10%)
    Snow with the probability 0.3 (30%)
    Sunny with the probability 0.6 (60%)

Using the estimates above, let us create a weather forecaster.

import java.util.ArrayList;
import java.util.Random;

public class WeatherForecaster {
    private Random random;

    public WeatherForecaster() {
        this.random = new Random();
    }

    public String forecastWeather() {
        double probability = this.random.nextDouble();

        if (probability <= 0.1) {
            return "Sleet";
        } else if (probability <= 0.4) { // 0.1 + 0.3
            return "Snow";
        } else { // the rest, 1.0 - 0.4 = 0.6
            return "Sunny";
        }
    }

    public int forecastTemperature() {
        return (int) ( 4 * this.random.nextGaussian() - 3 );
    }
}

The method forecastTemperature is interesting in many ways. Within this method, we are calling the method this.random.nextGaussian(), just like any other time we have called a method in the previous examples. Interestingly, this method of the class Random returns a value from the normal distribution (if you have no interest in the different varieties of random figures, that's okay!).

public int forecastTemperature() {
    return (int) ( 4 * this.random.nextGaussian() - 3 );
}

In the expression above, interesting is the section (int). This part of the expression changes the bracketed floating point number into an integer value. A corresponding method transforms integer values into floating point numbers: (double) integer. This is called an explicit type conversion.

Let us create a class with a main method that uses the class WeatherForecaster.

public class Program {

    public static void main(String[] args) {
        WeatherForecaster forecaster = new WeatherForecaster();

        // Use a list to help you organise things
        ArrayList<String> days = new ArrayList<String>();
        Collections.addAll(days, "Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun");

        System.out.println("Weather forecast for the next week:");
        for(String day : days) {
            String weatherForecast = forecaster.forecastWeather();
            int temperatureForecast = forecaster.forecastTemperature();

            System.out.println(day + ": " + weatherForecast + " " + temperatureForecast + " degrees.");
        }
    }
}

The printout from this program could be as follows:

Weather forecast for the next week:
Mon: Snow 1 degrees.
Tue: Snow 1 degrees.
Wed: Sunny -2 degrees.
Thu: Sunny 0 degrees.
Fri: Snow -3 degrees.
Sat: Snow -3 degrees.
Sun: Sunny -5 degrees.

Rolling the dice

In the template is class Dice that has the following functionality:

    The constructor Dice(int numberOfSides) creates a new dice object that has the amount of sides defined by the argument.
    The method roll tells the result of a roll (which depends on the number of its sides)

The frame of the program is as follows:

import java.util.Random;

public class Dice {
    private Random random;
    private int numberOfSides;

    public Dice(int numberOfSides){
        this.numberOfSides = numberofSides;
        random = new Random();

    }

    public int roll() {
          // we'll get a random number in the range 1-numberOfSides<
    }
}
    

Expand the class Dice so that with each roll the dice returns a random number between 1...number of sides. Here is a main program that tests the dice:

public class Program {
    public static void main(String[] args) {
        Dice dice = new Dice(6);

        int i = 0;
        while ( i < 10 ) {
            System.out.println( dice.roll() );
            i++;
        }
    }
}
    

The output could look something like this:

1
6
3
5
3
3
2
2
6
1
    

Password randomizer

Your assignment is to expand the class PasswordRandomizer that has the following functionality:

    The constructor PasswordRandomizer creates a new object, which uses the given password length.
    The method createPassword returns a new password, which consists of symbols a-z and is of the length given as a parameter to the constructor

The frame of the class is as follows:

import java.util.Random;

public class PasswordRandomizer {
    // Define the variables here

    public PasswordRandomizer(int length) {
        // Format the variable here
    }

    public String createPassword() {
      // Write the code here which returns the new password
    }
}
    

In the following is a program that uses a PasswordRandomizer object:

public
class Program {
    public static void main(String[] args) {
        PasswordRandomizer randomizer = new PasswordRandomizer(13);
        System.out.println("Password: " + randomizer.createPassword());
        System.out.println("Password: " + randomizer.createPassword());
        System.out.println("Password: " + randomizer.createPassword());
        System.out.println("Password: " + randomizer.createPassword());
    }
}
    

The output could look something like this:

Password: mcllsoompezvs
Password: urcxboisknkme
Password: dzaccatonjcqu
Password: bpqmedlbqaopq
    

Tip 1: this is how you turn the integer number into a character:

int number = 17;
char symbol = "abcdefghijklmnopqrstuvwxyz".charAt(number);
    

Tip 2: The tip in assignment 58 might be useful in this one too.
Lottery

Your assignment is to expand the class LotteryNumbers, which draws the lottery numbers of the week. The numbers of the week consist of 7 different numbers between 1 and 39. The class has the following functionality:

    the constructor LotteryNumbers creates a new LotteryNumbers object, which contains the new drawn numbers
    the method numbers returns the drawn numbers of this draw
    the method drawNumbers draws new numbers
    the method containsNumber reveals if the number is among the drawn numbers

The frame of the class is as follows:

import java.util.ArrayList;
import java.util.Random;

public class LotteryNumbers {
    private ArrayList<Integert> numbers;

    public LotteryNumbers() {
        // We'll format a list for the numbers
        this.numbers = new ArrayList<Integert>();
        // Draw numbers as LotteryNumbers is created
        this.drawNumbers();
    }

    public ArrayList<Integert> numbers() {
        return this.numbers;
    }

    public void drawNumbers() {
        // Write the number drawing here using the method containsNumber()
    }

    public boolean containsNumber(int number) {
        // Test here if the number is already among the drawn numbers
    }
}
    

The following main program comes with the template:

import java.util.ArrayList;

public class Program {
    public static void main(String[] args) {
        LotteryNumbers lotteryNumbers = new LotteryNumbers();
        ArrayList<Integert> numbers = lotteryNumbers.numbers();

        System.out.println("Lottery numbers:");
        for (int number : numbers) {
            System.out.print(number + " ");
        }
        System.out.println("");
    }
}
    

The program can print lines like these:

Lottery numbers:
3 5 10 14 15 27 37
    

Lottery numbers:
2 9 11 18 23 32 34
    

Note! a number can be in one set of numbers only once (per draw of course).
Game logic for Hangman

Your Finnish friend designed a Hangman game that looks like the following:

Your friend has programmed the user interface and also a skeleton for the game logic. Now, she asks you to finish the remaining pieces of the game logic.

The Finnish words sana, virheitä, viesti, hävisit and arvatut (kirjaimet) translate into word, (number of) faults, message, you lost and guessed (letters) respectively.

Amongst other stuff, with TMC you get the following skeleton for the class HangmanLogic

public class HangmanLogic {

    private String word;
    private String guessedLetters;
    private int numberOfFaults;

    public HangmanLogic(String word) {
        this.word = word.toUpperCase();
        this.guessedLetters = "";
        this.numberOfFaults = 0;
    }

    public int numberOfFaults() {
        return this.numberOfFaults;
    }

    public String guessedLetters() {
        return this.guessedLetters;
    }

    public int losingFaultAmount() {
        return 12;
    }

    public void guessLetter(String letter) {
        // program here the functionality for making a guess

        // if the letter has already been guessed, nothing happens

        // it the word does not contains the guessed letter, the number of faults increases
        // the letter is added among the already guessed letters
    }

    public String hiddenWord() {
        // program here the functionality for building the hidden word

        // create the hidden word by iterating through this.word letter by letter
        // if the letter in turn is within the guessed words, put it in the hidden word
        // if the letter is not among the guessed ones, replace it with _ in the hidden word

        // return the hidden word at the end

        return "";
    }
}
    

In this assignment, you should only touch class HangmanLogic and implement the functionality of the methods guessLetter(String letter) and hiddenWord().

Testing the code

The TMC project includes two classes that help you with testing. The class Main starts the graphical version of the game. The class TestProgram can be used to test the class HangmanLogic.
Guessing a letter

Touch only the method guessLetter(String letter) in this assignment!

When a user guesses a letter, the user interface calls method guessLetter which is supposed to take care of action related to guessing a letter. First, it should check if the letter has already been guessed. In that case, the method does not do anything.

The method increases the number of faults (this.numberOfFaults) if the word (this.word) does not contain the guessed letter. Then the letter is added among the already guessed letters (the object variable this.guessedLetters).

An example of how the method guessLetter should work:

HangmanLogic l = new HangmanLogic("kissa");
System.out.println("guessing: A, D, S, F, D");
l.guessLetter("A");   // correct
l.guessLetter("D");   // wrong
l.guessLetter("S");   // correct
l.guessLetter("F");   // wrong
l.guessLetter("D");   // This should not have any effect on the number of faults since D was already guessed
System.out.println("guessed letters: "+l.guessedLetters());
System.out.println("number of faults: "+l.numberOfFaults());
    

guessing: A, D, S, F, D
guessed letters: ADSF
number of faults: 2
    

Creating the hidden word

The Hangman user interface shows a hidden version of the word to the user. In the above figure, the hidden word is METO_I. All the letters that the user has already guessed are shown in the hidden word but the rest of the letters are replaced with underscores. In this part of the assignment, you should complete the method hiddenWord of Hangman logic that takes care of building the hidden word for the user interface.

Commands while, charAt and contains might be useful here. Note that a single char can be made into a string as follows:

char c = 'a';
String aString = "" + c;
    

An example of how the method works:

HangmanLogic l = new HangmanLogic("kissa");
System.out.println("word is: "+l.hiddenWord());

System.out.println("guessing: A, D, S, F, D");
l.guessLetter("A");
l.guessLetter("D");
l.guessLetter("S");
l.guessLetter("F");
l.guessLetter("D");
System.out.println("guessed letters: "+l.guessedLetters());
System.out.println("number of faults: "+l.numberOfFaults());
System.out.println("word now: "+l.hiddenWord());
    

word is: _____
guessing: A, D, S, F, D
guessed letters: ADSF
number of faults: 2
word now: __SSA
    

Now, you can test the game by using class Main. You can change the guessed word by changing the constructor parameter of the game logic:

HangmanLogic logic = new HangmanLogic("parameter");
HangmanUI game = new HangmanUI(logic);
game.start();
    

The game is played with the keyboard. You can end the game by pressing x in the upper left corner of the game window.

-------------------------------------------------------------------------------------------------------------------------------

More about objects and classes
Multiple constructors

Let us return to the class that handles Persons again. The class Person currently looks like this:

public class Person {

    private String name;
    private int age;
    private int height;
    private int weight;

     public Person(String name) {
        this.name = name;
        this.age = 0;
        this.weight = 0;
        this.height = 0;
    }

    public void printPerson() {
        System.out.println(this.name + " I am " + this.age + " years old");
    }

    public void becomeOlder() {
        this.age++;
    }

    public boolean adult(){
        if ( this.age < 18 ) {
            return false;
        }

        return true;
    }

    public double weightIndex(){
        double heightInMeters = this.height/100.0;

        return this.weight / (heightInMeters*heightInMeters);
    }

    public String toString(){
        return this.name + " I am " + this.age + " years old, my weight index is " + this.weightindex();
    }

    public void setHeight(int height){
        this.height = height;
    }

    public int getHeight(){
        return this.height;
    }

    public int getWeight() {
        return this.weight;
    }

    public void setWeight(int weight) {
        this.weight = weight;
    }

    public String getName(){
        return this.name;
    }
}

All person objects are 0 years old at creation, since the constructor sets it to 0:

public Person(String name) {
    this.name = name;
    this.age = 0;
    this.weight = 0;
    this.height = 0;
}

We also want to create a person so that in addition to name, can be given an age as a parameter. This can be achieved easily, since multiple constructors can exist. Let us make an alternative constructor. You do not need to remove the old one.

public Person(String name) {
    this.name = name;
    this.age = 0;
    this.weight = 0;
    this.height = 0;
}

public Person(String name, int age) {
    this.name = name;
    this.age = age;
    this.weight = 0;
    this.height = 0;
}

Now, creating objects can be done in two different ways:

public static void main(String[] args) {
    Person pekka = new Person("Pekka", 24);
    Person esko = new Person("Esko");

    System.out.println( pekka );
    System.out.println( esko );
}

Pekka, age 24 years
Esko, age 0 years

The technique in which a class has two constructors is called constructor overloading. A class can have multiple constructors, which are different from one another according to parameter quanitities and/or types. However, it is not possible to create two different constructors that have exactly the same type of parameters. We cannot add a constructor public Person(String name, int weight) on top of the old ones, since it is impossible for Java to tell the difference between this one and the one in which the integer stands for the age.
Calling your own constructor

But wait, in chapter 21 we noted that "copy-paste" code is not too great of an idea! When we inspect the overloaded constructors above, we notice that they have the same code repeated in them. We are not ok with this.

The old constructor actually is a special case of the new constructor. What if the old constructor could 'call' the new constructor? This can be done, since you can call another constructor from within a constructor with this!

Let us change the old constructor that does nothing, but only calls the new constructor below it and asks it to set the age to 0:

public Person(String name) {
    this(name, 0);  // run here the other constructor's code and set the age parameter to 0
}

public Person(String name, int age) {
    this.name = name;
    this.age = age;
    this.weight = 0;
    this.height = 0;
}

Calling the own constructor of a class this(name, 0); might seem a little peculiar. But we can imagine that during the call it will automatically copy-paste the code from the constructor below and that 0 is entered to the age parameter.
Overloading a method

Just like constructors, methods can also be overloaded and multiple versions of a method can exist. Again, the parameter types of different versions have to be different. Let us create another version of the becomeOlder, which enables aging the person the amount of years that is entered as a parameter:

public void becomeOlder() {
    this.age = this.age + 1;
}

public void becomeOlder(int years) {
    this.age = this.age + years;
}

In the following, "Pekka" is born as a 24-year old, ages one year, and then 10:

public static void main(String[] args) {
    Person pekka = new Person("Pekka", 24);

    System.out.println(pekka);
    pekka.becomeOlder();
    System.out.println(pekka);
    pekka.becomeOlder(10);
    System.out.println(pekka);
}

Prints:

Pekka, age 24 years
Pekka, age 25 years
Pekka, age 35 years

Now, a person has two becomeOlder methods. The method that is chosen to be run depends on the amount of parameters entered in to the method call. The method becomeOlder can also be run through the method becomeOlder(int years):

public void becomeOlder() {
    this.becomeOlder(1);
}

public void becomeOlder(int years) {
    this.age = this.age + years;
}

Overloaded counter
Multiple constructors

Make a class Counter that holds a number that can be decreased and increased. The counter also has an optional check that prevents the counter from going below 0. The class has to have the following constructors:

    public Counter(int startingValue, boolean check) creates a new counter with the given value. The check is on if the parameter given to check was true.
    public Counter(int startingValue) creates a new counter with the given value. The check on the new counter should be off.
    public Counter(boolean check) creates a new counter with the starting value 0. The check is on if the parameter given to check was true.
    public Counter() creates a new counter with the starting value of 0 and with checking off.

and the following methods:

    public int value() returns the current value of the counter
    public void increase() increases the value of the counter by one
    public void decrease() decreases the value of the counter by one, but not below 0 if the check is on

Alternative methods

Create also a one parametered versions of the methods increase and decrease:

    public void increase(int increaseAmount) increases the value by the amount of the parameter. If the value of the parameter is negative, the value will not change.
    public void decrease(int decreaseAmount) decreases the value of the counter by the amount given by the parameter, but not below 0 if the check is on. If the value of the parameter is negative, the value of the counter will not change.

Object is at the end of a wire

In chapter 20, we noted that ArrayList is at the end of a wire. Also objects are 'at the end of a wire'. What does this mean? Let us inspect the following example:

public static void main(String[] args) {
    Person pekka = new Person("Pekka", 24);

    System.out.println( pekka );
}

When we run the sentence Person pekka = new Person("Pekka", 24); an object is born. The object can be accessed through the variable pekka. Technically speaking, the object is not within the variable pekka (in the box 'pekka'), but pekka refers to the object that was born. In other words, the object is 'at the end of a wire' that is attached to a variable named pekka. The concept could be visualized like this:

Let us add to the program a variable person of the type Person and set its starting value to pekka. What happens now?

public static void main(String[] args) {
    Person pekka = new Person("Pekka", 24);

    System.out.println( pekka );

    Person person = pekka;
    person.becomeOlder(25);

    System.out.println( pekka );
}

Prints:

Pekka, age 24 years
Pekka, age 49 years

In the beginning, Pekka was 24 years old. Then a Person object at the end of a wire attached to a Person variable is aged by 25 years and as a consequence of that Pekka becomes older! What is going on here?

The command Person person = pekka; makes person refer to the same object that pekka refers to. So, a copy of the object is not born, but instead both of the variables refer to the same object. With the command Person person = pekka; a copy of the wire is born. The same thing as a picture (Note: in the picture p refers to the variable pekka, and h to the variable person in the main program. The variable names have also been abbreviated in some of the following pictures.):

In the example, "an unknown person steals Pekka's identity". In the following, we have expanded the example so that a new object is created and pekka begins to refer to a new object:

public static void main(String[] args) {
    Person pekka = new Person("Pekka", 24);

    System.out.println( pekka );

    Person person = pekka;
    person.becomeOlder(25);

    System.out.println( pekka );

    pekka = new Person("Pekka Mikkola", 24);
    System.out.println( pekka );
}

Prints:

Pekka, age 24 years
Pekka, age 49 years
Pekka Mikkola, age 24 years

The variable pekka refers to one object, but then begins to refer to another. Here is the situation after running the previous line of code:

Let's develop the example further by making person to refer to 'nothing', to null:

public static void main(String[] args) {
    Person pekka = new Person("Pekka", 24);

    System.out.println( pekka );

    Person person = pekka;
    person.becomeOlder(25);

    System.out.println( pekka );

    pekka = new Person("Pekka Mikkola", 24);
    System.out.println( pekka );

    person = null;
    System.out.println( person );
}

After running that, the situation looks like this:

Nothing refers to the second object. The object has become 'garbage'. Java's garbace collector cleans up the garbage every now and then by itself. If this did not happen, the garbage would pile up in the computer's memory until the execution of the program is done.

We notice this on the last line whine we try to print 'nothing' (null) on the last line:

Pekka, age 24 years
Pekka, age 49 years
Pekka Mikkola, age 24 years
null

What happens if we try to call a "nothing's" method, for example the method weightIndex:

public static void main(String[] args) {
    Person pekka = new Person("Pekka", 24);

    System.out.println( pekka );

    Person person = null;
    System.out.println( person.weightIndex() );
}

Result:

Pekka, age 24 years
Exception in thread "main" java.lang.NullPointerException
        at Main.main(Main.java:20)
Java Result: 1

Not good. This might be the first time in your life that you see the text NullPointerException. But we can assure you that it will not be the last. NullPointerException is an exception state, when we try to call methods of an object with the value null.
An object as a method parameter

We have seen that a method can have, for example int, double, String or ArrayList as its parameter. ArrayLists and character strings are objects, so as one might guess a method can take any type of object as a parameter. Let us demonstrate this with an example.

People whose weight index exceeds a certain limit are accepted into the Weight Watchers. The limit is not the same in all Weight Watchers associations. Let us make a class corresponding to the Weight Watchers association. As the object is being created, the lowest acceptance limit is passed to the constructor as a parameter.

public class WeightWatchersAssociation {
    private double lowestWeightIndex;

    public WeightWatchersAssociation(double indexLimit) {
        this.lowestWeightIndex = indexLimit;
    }

}

Next we will create a method, with which we can check if a person is eligible to the association, in other words we check if a person's weight index is large enough. The method returns true if the person that is passed in as a parameter is eligible and false if not.

public class WeightWatchersAssociation {
    // ...

    public boolean isAcceptedAsMember(Person person) {
        if ( person.weightIndex() < this.lowestWeightIndex ) {
            return false;
        }

        return true;
    }
}

The method isAcceptedAsMember of the WeightWatchersAssociation object gets a Person object as its parameter (or more accurately the wire to the person), and then calls the method weightIndex of the person that it received as a parameter.

In the following, is a test main program in which a person object matti and a person object juhana is passed to the weight watchers association's method:

public static void main(String[] args) {
    Person matti = new Person("Matti");
    matti.setWeight(86);
    matti.setHeight(180);

    Person juhana = new Person("Juhana");
    juhana.setWeight(64);
    juhana.setHeight(172);

    WeightWatchersAssociation kumpulasWeight = new WeightWatchersAssociation(25);

    if ( kumpulasWeight.isAcceptedAsMember(matti) ) {
        System.out.println( matti.getName() + " is accepted as a member");
    } else {
        System.out.println( matti.getName() + " is not accepted as a member");
    }

    if ( kumpulasWeight.isAcceptedAsMember(juhana) ) {
        System.out.println( juhana.getName() + " is accepted as a memberksi");
    } else {
        System.out.println( juhana.getName() + " is not accepted as a member");
    }
}

The program prints:

Matti is accepted as a member
Juhana is not accepted as a member

A few NetBeans-tips

    All NetBeans-tips are found here
    The automatic generating of constructors, getters and setters.

    Go inside of the code block of the class, but outside of all methods and simultaneously press Ctrl+Space. If your class, for example, has an object variable balance, NetBeans will offer you the opportunity to generate the getter and setter methods, and a constructor that sets a starting value for the object variable.

Reformatory

In this assignment, we use the already given class Person and are supposed to build a new class Reformatory. Reformatory objects do certain things to persons, e.g. measure their weight and feed them.

Note: you should not alter the code in the class Person!
Weight of a person

The reformatory class already has a method skeleton public int weight(Person person):

public class Reformatory {

    public int weight(Person person) {
       // returns the weight of the parameter
       return -1;
    }
}
  

The method gets a person object as a parameter. The method is supposed to return the weight of the parameter, so the method should call a suitable method of person, get the return value and then return it to the caller.

In the following a reformatory weight's two persons:

public static void main(String[] args) {
    Reformatory eastHelsinkiReformatory = new Reformatory();

    Person brian = new Person("Brian", 1, 110, 7);
    Person pekka = new Person("Pekka", 33, 176, 85);

    System.out.println(brian.getName() + " weight: " + eastHelsinkiReformatory.weight(brian) + " kilos");
    System.out.println(pekka.getName() + " weight: " + eastHelsinkiReformatory.weight(pekka) + " kilos");
}
  

The output should be:

Brian weight: 7 kilos
Pekka weight: 85 kilos
  

Feeding a person

In the previous part of the assignment, the method weight queried some information from the parameter object by calling its method. It is also possible to change the state of the parameter. Add to class Reformatory the method public void feed(Person person) that increases the weight of its parameter by one.

Next, an example where first the weight of Pekka and Brian is measured and printed. Then Reformatory feeds Brian three times and after that the weights are measured and printed again.

public static void main(String[] args) {
    Reformatory eastHelsinkiReformatory = new Reformatory();

    Person brian = new Person("Brian", 1, 110, 7);
    Person pekka = new Person("Pekka", 33, 176, 85);

    System.out.println(brian.getName() + " weight: " + eastHelsinkiReformatory.weight(brian) + " kilos");
    System.out.println(pekka.getName() + " weight: " + eastHelsinkiReformatory.weight(pekka) + " kilos");

    eastHelsinkiReformatory.feed(brian);
    eastHelsinkiReformatory.feed(brian);
    eastHelsinkiReformatory.feed(brian);

    System.out.println("");

    System.out.println(brian.getName() + " weight: " + eastHelsinkiReformatory.weight(brian) + " kilos");
    System.out.println(pekka.getName() + " weight: " + eastHelsinkiReformatory.weight(pekka) + " kilos");
}
  

The output should reveal that Brian has gained 3 kilos:

Brian weight: 7 kilos
Pekka weight: 85 kilos

Brian weight: 10 kilos
Pekka weight: 85 kilos
  

Number of times a weight has been measured

Add to class Reformatory the method public int totalWeightsMeasured() that returns the total number of times a weight has been measured.

With the following main program:

public static void main(String[] args) {
    Reformatory eastHelsinkiReformatory = new Reformatory();

    Person brian = new Person("Brian", 1, 110, 7);
    Person pekka = new Person("Pekka", 33, 176, 85);

    System.out.println("total weights measured "+eastHelsinkiReformatory.totalWeightsMeasured());

    eastHelsinkiReformatory.weight(brian);
    eastHelsinkiReformatory.weight(pekka);

    System.out.println("total weights measured "+eastHelsinkiReformatory.totalWeightsMeasured());

    eastHelsinkiReformatory.weight(brian);
    eastHelsinkiReformatory.weight(brian);
    eastHelsinkiReformatory.weight(brian);
    eastHelsinkiReformatory.weight(brian);

    System.out.println("total weights measured "+eastHelsinkiReformatory.totalWeightsMeasured());
}
  

the output should be:

total weights measured 0
total weights measured 2
total weights measured 6
  

Lyyra card and Cash Register
The "stupid" Lyyra card

In the last set of exercises, we implemented the class LyyraCard. The card had methods for paying economical and gourmet lunches and a method for loading money.

Last week's version of the card is however somehow problematic. The card knew the lunch prices so that it could take the right price from the balance if a lunch was paid. What if the lunch prices change? Or what if it is decided that LyyraCards could also be used to purchase coffee? A change like these would mean that all the existing LyyraCards should be replaced with the new ones with the right prices and/or new methods. This does not sound good at all!

A better solution is to store only the balance on the card and have all the inteligence in a cash register.

We will soon program the cash register but let us start by completing the "stupid" version of the Lyyra card. The card holds the balance and has only two methods, public void loadMoney(double amount) that is already implemented and public boolean pay(double amount) that you should complete according to the instructions below:

public class LyyraCard {
    private double balance;

    public LyyraCard(double balance) {
        this.balance = balance;
    }

    public double balance() {
        return this.balance;
    }

    public void loadMoney(double amount) {
        this.balance += amount;
    }

    public boolean pay(double amount){
       // the method checks if the balance of the card is at least the amount given as parameter
       // if not, the method returns false meaning that the card could not be used for the payment
       // if the balance is enough, the given amount is taken from the balance and true is returned
    }
}
  

With the following main:

public class Main {
    public static void main(String[] args) {
        LyyraCard cardOfPekka = new LyyraCard(10);

        System.out.println("money on the card " + cardOfPekka.balance() );
        boolean succeeded = cardOfPekka.pay(8);
        System.out.println("money taken: " + succeeded );
        System.out.println("money on the card " + cardOfPekka.balance() );

        succeeded = cardOfPekka.pay(4);
        System.out.println("money taken: " + succeeded );
        System.out.println("money on the card " + cardOfPekka.balance() );
    }
}
  

the output should be

money on the card 10.0
money taken: true
money on the card 2.0
money taken: false
money on the card 2.0
  

Cash Register and paying with cash

In Unicafe, a client pays either with cash or with a Lyyra Card. The personnel uses a cash register to charge the client. Let us start by implementig the part of CashRegister that takes care of cash payments.

Below is the skeleton of CashRegister that also has the information on how the methods should be implemented:

public class CashRegister {
    private double cashInRegister;   // the amount of cash in the register
    private int economicalSold;      // the amount of economical lunches sold
    private int gourmetSold;         // the amount of gourmet lunches sold

    public CashRegister() {
        // at start the register has 1000 euros
    }

    public double payEconomical(double cashGiven) {
        // the price of the economical lunch is 2.50 euros
        // if the given cash is at least the price of the lunch:
        //    the price of lunch is added to register
        //    the amount of the sold lunches is incremented by one
        //    the method returns cashGiven - lunch price
        // if not enough money is given, all is returned and nothing else happens
    }

    public double payGourmet(double cashGiven) {
        // the price of the gourmet lunch is 4.00 euros
        // if the given cash is at least the price of the lunch:
        //    the price of lunch is added to the register
        //    the amount of the sold lunches is incremented by one
        //    the method returns cashGiven - lunch price
        // if not enough money is given, all is returned and nothing else happens
    }

    public String toString() {
        return "money in register "+cashInRegister+" economical lunches sold: "+economicalSold+" gourmet lunches sold: "+gourmetSold;
    }
}
  

When correctly implemented, the following main:

public class Main {
    public static void main(String[] args) {
        CashRegister unicafeExactum = new CashRegister();

        double theChange = unicafeExactum.payEconomical(10);
        System.out.println("the change was " + theChange );

        theChange = unicafeExactum.payEconomical(5);
        System.out.println("the change was "  + theChange );

        theChange = unicafeExactum.payGourmet(4);
        System.out.println("the change was "  + theChange );

        System.out.println( unicafeExactum );
    }
}
  

should output:

the change was 7.5
the change was 2.5
the change was 0.0
money in register 1009.0 economical lunches sold: 2 gourmet lunches sold: 1
  

Paying with card

Extend the cash register with methods to charge a lunch price from a Lyyra Card. See below how the methods should appear and behave:

public class CashRegister {
    // ...

    public boolean payEconomical(LyyraCard card) {
        // the price of the economical lunch is 2.50 euros
        // if the balance of the card is at least the price of the lunch:
        //    the amount of sold lunches is incremented by one
        //    the method returns true
        // if not, the method returns false
    }

    public boolean payGourmet(LyyraCard card) {
        // the price of the gourmet lunch is 4.00 euros
        // if the balance of the card is at least the price of the lunch:
        //    the amount of sold lunches is incremented by one
        //    the method returns true
        // if not, the method returns false
    }

    // ...
}
  

Note: card payments do not affect the amount of money in the register!

Example main and output:

public class Main {
    public static void main(String[] args) {
        CashRegister unicafeExactum = new CashRegister();

        double theChange = unicafeExactum.payEconomical(10);
        System.out.println("the change was " + theChange );

        LyyraCard cardOfJim = new LyyraCard(7);

        boolean succeeded = unicafeExactum.payGourmet(cardOfJim);
        System.out.println("payment success: " + succeeded);
        succeeded = unicafeExactum.payGourmet(cardOfJim);
        System.out.println("payment success: " + succeeded);
        succeeded = unicafeExactum.payEconomical(cardOfJim);
        System.out.println("payment success: " + succeeded);

        System.out.println( unicafeExactum );
    }
}
  

the change was 7.5
payment success: true
payment success: false
payment success: true
money in register 1002.5 economical lunches sold: 2 gourmet lunches sold: 1
  

Loading money

To complete the assignment, extend the cash register with a method that can be used to load cash to Lyyra Cards. When a certain amount is loaded to the card, the amount stored in the register increases correspondingly. Remember that the amount to be loaded needs to be positive! The method skeleton:

public void loadMoneyToCard(LyyraCard card, double sum) {
   // ...
}
  

Example main and its output:

public class Main {
    public static void main(String[] args) {
        CashRegister unicafeExactum = new CashRegister();
        System.out.println( unicafeExactum );

        LyyraCard cardOfJim = new LyyraCard(2);

        System.out.println("the card balance " + cardOfJim.balance() + " euros");

        boolean succeeded = unicafeExactum.payGourmet(cardOfJim);
        System.out.println("payment success: " + succeeded);

        unicafeExactum.loadMoneyToCard(cardOfJim, 100);

        succeeded = unicafeExactum.payGourmet(cardOfJim);
        System.out.println("payment success: " + succeeded);

        System.out.println("the card balance " + cardOfJim.balance() + " euros");

        System.out.println( unicafeExactum );
    }
}
  

money in register 1000.0 economical lunches sold: 0 gourmet lunches sold: 0
money on the card 2.0 euros
payment success: false
payment success: true
the card balance 98.0 euros
money in register 1100.0 economical lunches sold: 0 gourmet lunches sold: 1
  

Another object of the same type as a parameter to a method

We will keep on working with the Person class. As we recall, persons know their age:

public class Person {

    private String name;
    private int age;
    private int height;
    private int weight;

    // ...
}

We want to compare ages of two persons. The comparison can be done in a number of ways. We could define a getter method getAge for a person. Comparing two persons in that case would be done like this:

Person pekka = new Person("Pekka");
Person juhana = new Person("Juhana")

if ( pekka.getAge() > juhana.getAge() ) {
    System.out.println(pekka.getName() + " is older than " + juhana.getName());
}

We will learn a slightly more object-oriented way to compare the ages of two people.

We will create a method boolean olderThan(Person compared) for the Person class, with which we can compare a certain person with a person that is given as a parameter.

The method is meant to be used in the following way:

public static void main(String[] args) {
    Person pekka = new Person("Pekka", 24);
    Person antti = new Person("Antti", 22);

    if (pekka.olderThan(antti)) {  //  same as pekka.olderThan(antti)==true
        System.out.println(pekka.getName() + " is older than " + antti.getName());
    } else {
        System.out.println(pekka.getName() + " isn't older than " + antti.getName());
    }
}

Here, we ask Pekka if he is older than Antti, Pekka replies true if he is, and false if he is not. In practice, we call the method olderThan of the object that pekka refers to. For this method, we give as a parameter the object that antti refers to.

The program prints:

Pekka is older than Antti

The program gets a person object as its parameter (or more accurately a reference to a person object, which is at 'the end of a wire') and then compares its own age this.age to the age of the compared compared.age. The implementation looks like this:

public class Person {
    // ...

    public boolean olderThan(Person compared) {
        if ( this.age > compared.age ) {
            return true;
        }

        return false;
    }
}

Even though age is a private object variable, we can read the value of the variable by writing compared.age. This is because private variables can be read in all methods that the class in question contains. Note that the syntax resembles the call of a method of an object. Unlike calling a method, we refer to a field of an object, in which case we do not write the parentheses.
The date as an object

Another example of the same theme. Let us create a class, which can represent dates.

Within an object, the date is represented with three object variables. Let us also make a method, which can compare whether the date is earlier than a date that is given as a parameter:

public class MyDate {
    private int day;
    private int month;
    private int year;

    public MyDate(int day, int month, int year) {
        this.day = day;
        this.month = month;
        this.year = year;
    }

    public String toString() {
        return this.day + "." + this.month + "." + this.year;
    }

    public boolean earlier(MyDate compared) {
        // first we'll compare years
        if ( this.year < compared.year ) {
            return true;
        }

        // if the years are the same, we'll compare the months
        if ( this.year == compared.year && this.month < compared.month ) {
            return true;
        }

        // years and months the same, we'll compare the days
        if ( this.year == compared.year && this.month == compared.month &&
                this.day < compared.day ) {
            return true;
        }

        return false;
    }
}

Example of usage:

public static void main(String[] args) {
    MyDate p1 = new MyDate(14, 2, 2011);
    MyDate p2 = new MyDate(21, 2, 2011);
    MyDate p3 = new MyDate(1, 3, 2011);
    MyDate p4 = new MyDate(31, 12, 2010);

    System.out.println( p1 + " earlier than " + p2 + ": " + p1.earlier(p2));
    System.out.println( p2 + " earlier than " + p1 + ": " + p2.earlier(p1));

    System.out.println( p2 + " earlier than " + p3 + ": " + p2.earlier(p3));
    System.out.println( p3 + " earlier than " + p2 + ": " + p3.earlier(p2));

    System.out.println( p4 + " earlier than " + p1 + ": " + p4.earlier(p1));
    System.out.println( p1 + " earlier than " + p4 + ": " + p1.earlier(p4));
}

14.2.2011 earlier than 21.2.2011: true
21.2.2011 earlier than 14.2.2011: false
21.2.2011 earlier than 1.3.2011: true
1.3.2011 earlier than 21.2.2011: false
31.12.2010 earlier than 14.2.2011: true
14.2.2011 earlier than 31.12.2010: false

Apartment comparison

The information system of a Housing service represents the apartments it has for sale using objects of the following class:

public class Apartment {
    private int rooms;
    private int squareMeters;
    private int pricePerSquareMeter;

    public Apartment(int rooms, int squareMeters, int pricePerSquareMeter){
        this.rooms = rooms;
        this.squareMeters = squareMeters;
        this.pricePerSquareMeter = pricePerSquareMeter;
    }
}
  

Next you should implement a couple of methods that help in apartment comparisons.
Larger

Implement the method public boolean larger(Apartment otherApartment) that returns true if the Apartment object for which the method is called (this) is larger than the apartment object given as parameter (otherApartment).

Example of the usage:

Apartment studioManhattan = new Apartment(1, 16, 5500);
Apartment twoRoomsBrooklyn = new Apartment(2, 38, 4200);
Apartment fourAndKitchenBronx = new Apartment(3, 78, 2500);

System.out.println( studioManhattan.larger(twoRoomsBrooklyn) );       // false
System.out.println( fourAndKitchenBronx.larger(twoRoomsBrooklyn) );   // true
  

Price difference

Implement the method public int priceDifference(Apartment otherApartment) that returns the absolute value of the price difference of the Apartment object for which the method is called (this) and the apartment object given as parameter (otherApartment). The price of an apartment is squareMeters * pricePerSquareMeter.

Example of the usage:

Apartment studioManhattan = new Apartment(1, 16, 5500);
Apartment twoRoomsBrooklyn = new Apartment(2, 38, 4200);
Apartment fourAndKitchenBronx = new Apartment(3, 78, 2500);

System.out.println( studioManhattan.priceDifference(twoRoomsBrooklyn) );        // 71600
System.out.println( fourAndKitchenBronx.priceDifference(twoRoomsBrooklyn) );    // 35400
  

more expensive than

Implement the method public boolean moreExpensiveThan(Apartment otherApartment) that returns true if the Apartment-object for which the method is called (this) has a higher price than the apartment object given as parameter (otherApartment).

Example of the usage:

Apartment studioManhattan = new Apartment(1, 16, 5500);
Apartment twoRoomsBrooklyn = new Apartment(2, 38, 4200);
Apartment fourAndKitchenBronx = new Apartment(3, 78, 2500);

System.out.println( studioManhattan.moreExpensiveThan(twoRoomsBrooklyn) );       // false
System.out.println( fourAndKitchenBronx.moreExpensiveThan(twoRoomsBrooklyn) );   // true
  

Objects on a list

We've used ArrayLists in a lot of examples and assignments already. You can add character strings, for example, to an ArrayList object and going through the strings, searching, removing and sorting them and so forth, are painless actions.

You can put any type of objects in ArrayLists. Let's create a person list, an ArrayList<Person> and put a few person objects in it:

public static void main(String[] args) {
    ArrayList<Person> teachers = new ArrayList<Person>();

    // first we can take a person into a variable
    Person teacher = new Person("Juhana");
    // and then add it to the list
    teachers.add(teacher);

    // or we can create the object as we add it:
    teachers.add( new Person("Matti") );
    teachers.add( new Person("Martin") );

    System.out.println("teachers as newborns: ");
    for ( Person prs : teachers ) {
        System.out.println( prs );
    }

    for ( Person prs : teachers ) {
        prs.becomeOlder( 30 );
    }

    System.out.println("in 30 years: ");
    for ( Person prs : teachers ) {
        System.out.println( prs );
    }
}

The program prints:

teachers as newborns:
Juhana, age 0 years
Matti, age 0 years
Martin, age 0 years
in 30 years:
Juhana, age 30 years
Matti, age 30 years
Martin, age 30 years

Students
Class Student

Implement class Student that holds the following information about a student:

    name (String)
    studentNumber (String)

The class should have the following methods:

    A constructor that initializes the name and the student number with the given parameters.
    getName, that returns the student name
    getStudentNumber, that returns the student number
    toString, that returns a String representation of the form: Pekka Mikkola (013141590)

With the following code:

public class Main {
    public static void main(String[] args) {
        Student pekka = new Student("Pekka Mikkola", "013141590");
        System.out.println("name: " + pekka.getName());
        System.out.println("studentnumber: " + pekka.getStudentNumber());
        System.out.println(pekka);
    }
}
  

The output should be:

name: Pekka Mikkola
studentnumber: 013141590
Pekka Mikkola (013141590)
  

List of students

Implement a main program that works as follws:

name: Alan Turing
studentnumber: 017635727
name: Linus Torvalds
studentnumber: 011288989
name: Steve Jobs
studentnumber: 013672548
name:

Alan Turing (017635727)
Linus Torvalds (011288989)
Steve Jobs (013672548)
  

So the program asks for student information from the user until the user gives a student an empty name. After the student info has been enteres, all the students are printed. From each inputted name-studentnumber-pair, the program should create a Student object. The program should store the students in an ArrayList which is defined as follows:

ArrayList<Student> list = new ArrayList<Student>();
  

Search

Extend the program of the previous part so that after the student info has been entered and students printed, the user can search the student list based on a given search term. The extended program should work in the following manner:

name: Carl Gustaf Mannerheim
studentnumber: 015696234
name: Steve Jobs
studentnumber: 013672548
name: Edsger Dijkstra
studentnumber: 014662803
name:

Carl Gustaf Mannerheim (015696234)
Steve Jobs (013672548)
Edsger Dijkstra (014662803)

Give search term: st
Result:
Carl Gustaf Mannerheim (015696234)
Edsger Dijkstra (014662803)
  

TIP: in the search you should iterate (using for or while) through the student list and by using the method contains of String check if a student's name (obtained with method getName) matches the search term.
An object within an object

Objects can have objects within them, not only character strings but also self-defined objects. Let's get back to the Person-class again and add a birthday for the person. We can use the MyDate-object we created earlier here:

public class Person {
    private String name;
    private int age;
    private int weight;
    private int height;
    private MyDate birthMyDate;

    // ...

Let's create a new constructor for persons, which enables setting a birthday:

    public Person(String name, int day, int month, int year) {
        this.name = name;
        this.weight = 0;
        this.height = 0;
        this.birthMyDate = new MyDate(day, month, year);
    }

So because the parts of the date are given as constructor parameters (day, month, year), the date object is created out of them and then inserted to the object variable birthMyDate.

Let's edit toString so that instead of age, it displays the birthdate:

public String toString() {
    return this.name + ", born " + this.birthMyDate;
}

And then let's test how the renewed Person class works:

public static void main(String[] args) {
    Person martin = new Person("Martin", 24, 4, 1983);

    Person juhana = new Person("Juhana", 17, 9, 1985);

    System.out.println( martin );
    System.out.println( juhana );
}

Prints:

Martin, born 24.4.1983
Juhana, born 17.9.1985

In chapter 24.4, we noted that objects are 'at the end of a wire'. Take a look at that chapter again for good measure.

Person objects have the object variables name, which is a String-object and birthMyDate, which is a MyDate object. The variables of person are consequently both objects, so technically speaking they don't actually exist within a person object, but are 'at the end of a wire'. In other words a person has a reference to the objects stored in its object variables. The concept as a picture:

The main program now has two person programs at the ends of wires. The persons have a name and a birthdate. Because both are objects, both are at the ends of wires the person holds.

Birthday seems like a good expansion to the Person class. We notice, however, that the object variable age is becoming obsolete and should probably be removed since the age can be determined easily with the help of the current date and birthday. In Java, the current day can be figured out, for example, like this:

int day = Calendar.getInstance().get(Calendar.DATE);
int month = Calendar.getInstance().get(Calendar.MONTH) + 1; // January is 0 so we add 1
int year = Calendar.getInstance().get(Calendar.YEAR);
System.out.println("Today is " + day + "." + month + "." + year );

When age is removed, the olderThan method has to be changed so that it compares birthdates. We'll do this as an excersise assignment.
Clock object

In assignment 78 we used objects of the class BoundedCounter to implement a clock in the main method. In this assignment we will tranform the clock to an object. The skeleton of the class clock looks like the following:

public class Clock {
    private BoundedCounter hours;
    private BoundedCounter minutes;
    private BoundedCounter seconds;

    public Clock(int hoursAtBeginning, int minutesAtBeginning, int secondsAtBeginning) {
      // the counters that represent hours, minutes and seconds are created and
      // set to have the correct initial values
    }

    public void tick(){
      // Clock advances by one second
    }

    public String toString() {
        // returns the string representation
    }
}
  

Copy the class BoundedCounter from assignment 78 to the project of this assignment!

Implement constructor and method tick for the class Clock. Use the following main to test your clock:

public class Main {
    public static void main(String[] args) {
        Clock clock = new Clock(23, 59, 50);

        int i = 0;
        while( i < 20) {
            System.out.println( clock );
            clock.tick();
            i++;
        }
    }
}
  

The output should be:

23:59:50
23:59:51
23:59:52
23:59:53
23:59:54
23:59:55
23:59:56
23:59:57
23:59:58
23:59:59
00:00:00
00:00:01
...
  

A list of objects within an object

Let's expand the WeightWatchersAssociation object so that the association records all its members into an ArrayList object. So in this case the list will be filled with Person objects. In the extended version the association is given a name as a constructor parameter:

public class WeightWatchersAssociation {
    private double lowestWeightIndex;
    private String name;
    private ArrayList<Person> members;

    public WeightWatchersAssociation(String name, double lowestWeightIndex) {
        this.lowestWeightIndex = lowestWeightIndex;
        this.name = name;
        this.members = new ArrayList<Person>();
    }

    //..
}

Let's create a method with which a person is added to the association. The method won't add anyone to the association but people with a high enough weight index. Let's also make a toString with which the members' names are printed:

public class WeightWatchersAssociation {
    // ...

    public boolean isAccepted(Person person) {
        if ( person.weightIndex() < this.lowestWeightIndex ) {
            return false;
        }

        return true;
    }

    public void addAsMember(Person person) {
        if ( !isAccepted(person) ) { // same as isAccepted(person) == false
            return;
        }

        this.members.add(person);
    }

    public String toString() {
        String membersAsString = "";

        for ( Person member : this.members ) {
            membersAsString += "  " + member.getName() + "\n";
        }

        return "Weightwatchers association " + this.name + " members: \n" + membersAsString;
    }
}

The method addAsMember uses the method isAccepted that was creater earlier.

Let's try out the expanded weightwatchers association:

public static void main(String[] args) {
    WeightWatchersAssociation weightWatcher = new WeightWatchersAssociation("Kumpulan paino", 25);

    Person matti = new Person("Matti");
    matti.setWeight(86);
    matti.setHeight(180);
    weightWatcher.addAsMember(matti);

    Person juhana = new Person("Juhana");
    juhana.setWeight(64);
    juhana.setHeight(172);
    weightWatcher.addAsMember(juhana);

    Person harri = new Person("Harri");
    harri.setWeight(104);
    harri.setHeight(182);
    weightWatcher.addAsMember(harri);

    Person petri = new Person("Petri");
    petri.setWeight(112);
    petri.setHeight(173);
    weightWatcher.addAsMember(petri);

    System.out.println( weightWatcher );
}

In the output we can see that Juhana wasn't accepted as a member:

The members of weight watchers association 'kumpulan paino':
  Matti
  Harri
  Petri

Team and Players
Class Team

Implement a class Team. At this stage team has only a name (String) and the following functionality:

    a constructor that sets the team name
    getName, that returns the name

With the code:

public class Main {
    public static void main(String[] args) {
    Team barcelona = new Team("FC Barcelona");
    System.out.println("Team: " + barcelona.getName());
    }
}
  

the output should be::

Team: FC Barcelona
  

Player

Create a class Player with the instance variables for the player name and the amount of goals. A player should have two constructors: one that initializes the name and an another that initializes the name and the amount of goals. Implement also the following methods:

    getName, returns the player name
    goals, returns the amount of goals
    toString, returns a string representation that is formed as in the example below

Example usage:

public class Main {
    public static void main(String[] args) {
    Team barcelona = new Team("FC Barcelona");
    System.out.println("Team: " + barcelona.getName());

        Player brian = new Player("Brian");
        System.out.println("Player: " + brian);

        Player pekka = new Player("Pekka", 39);
        System.out.println("Player: " + pekka);
    }
}
  

and the expected output:

Team: FC Barcelona
Player: Brian, goals 0
Player: Pekka, goals 39
  

Adding players to a team

Add to the class Team the following methods:

    addPlayer, adds a player to the team
    printPlayers, prints the players in the team

You should store the players to an instance variable of the type ArrayList<Player> within the class Team.

With the code:

public class Main {
    public static void main(String[] args) {
    Team barcelona = new Team("FC Barcelona");

        Player brian = new Player("Brian");
        Player pekka = new Player("Pekka", 39);

        barcelona.addPlayer(brian);
        barcelona.addPlayer(pekka);
        barcelona.addPlayer(new Player("Mikael", 1)); // works similarly as the above

        barcelona.printPlayers();
    }
}
  

the output should be:

Brian, goals 0
Pekka, goals 39
Mikael, goals 1
  

The team maximum size and current size

Add to the class Team the methods

    setMaxSize(int maxSize), sets the maximum number of players that the team can have
    size, returns the number of players in the team

By default the maximum number of players should be set to 16, and that can be changed with the method setMaxSize. Change the method addPlayer so that it does not add players to the team if the team already has the maximum number of players.

With the code:

public class Main {
    public static void main(String[] args) {
    Team barcelona = new Team("FC Barcelona");
        barcelona.setMaxSize(1);

        Player brian = new Player("Brian");
        Player pekka = new Player("Pekka", 39);
        barcelona.addPlayer(brian);
        barcelona.addPlayer(pekka);
        barcelona.addPlayer(new Player("Mikael", 1)); // works similarly as the above

        System.out.println("Number of players: " + barcelona.size());
    }
}
  

the output should be

Number of players: 1
  

Goals of a team

Add to the class Team the method

    goals, returns the total number of goals for all the players in the team

With the code:

public class Main {
    public static void main(String[] args) {
        Team barcelona = new Team("FC Barcelona");

        Player brian = new Player("Brian");
        Player pekka = new Player("Pekka", 39);
        barcelona.addPlayer(brian);
        barcelona.addPlayer(pekka);
        barcelona.addPlayer(new Player("Mikael", 1)); // works similarly as the above

        System.out.println("Total goals: " + barcelona.goals());
    }
}
  

the output should be

Total goals: 40
  

Method returns an object

We've seen methods that return booleans, numbers, lists and strings. It's easy to guess that a method can return any type of an object. Let's make a method for the weight watchers association that returns the person with the highest weight index.

public class WeightWatchersAssociation {
    // ...

    public Person personWithHighestWeightIndex() {
        // if members list is empty, we'll return null-reference
        if ( this.members.isEmpty() ) {
            return null;
        }

        Person heaviestSoFar = this.members.get(0);

        for ( Person person : this.members) {
            if ( person.weightIndex() > heaviestSoFar.weightIndex() ) {
                heaviestSoFar = person;
            }
        }

        return heaviestSoFar;
    }
}

The logic in this method works in the same way as when finding the largest number in a list. We use a dummy variable heaviestSoFar which is initially made to refer to the first person on the list. After that the list is read through and we see if there's anyone with a greater weight index in it, if so, we make heaviestSoFar refer to that one instead. At the end we return the value of the dummy variable, or in other words the reference to a person object.

Let's make an expansion to the previous main program. The main program receives the reference returned by the method to its variable heaviest.

public static void main(String[] args) {
    WeightWatchersAssociation weightWatcher = new WeightWatchersAssociation("Kumpluan paino", 25);

    // ..

    Person heaviest = weightWatcher.personWithHighestWeightIndex();
    System.out.print("member with the greatest weight index: " + heaviest.getName() );
    System.out.println(" weight index " + String.format( "%.2f", heaviest.weightIndex() ) );
}

Prints:

member with the greatest weight index: Petri
weight index 37,42

Method returns an object it creates

In the last example a method returned one Person object that the WeightWatcers object had in it. It's also possible that a method returns an entirely new object. In the following is a simple counter that has a method clone with which a clone - an entirely new counter object - can be made from the counter, which at creation has the same value as the counter that is being cloned:

public Counter {
    private int value;

    public Counter(){
        this(0);
    }

    public Counter(int initialValue){
        this.value = initialValue;
    }

    public void grow(){
        this.value++;
    }

    public String toString(){
        return "value: "+value;
    }

    public Counter clone(){
        // lets create a new counter object, that gets as its initial value
        // the value of the counter that is being cloned
        Counter clone = new Counter(this.value);

        // return the clone to the caller
        return clone;
    }
}

Here's a usage example:

Counter counter = new Counter();
counter.grow();
counter.grow();

System.out.println(counter);         // prints 2

Counter clone = counter.clone();

System.out.println(counter);         // prints 2
System.out.println(clone);           // prints 2

counter.grow();
counter.grow();
counter.grow();
counter.grow();

System.out.println(counter);         // prints 6
System.out.println(clone);           // prints 2

clone.grow();

System.out.println(counter);         // prints 6
System.out.println(clone);           // prints 3

The value of the object being cloned and the value of the clone - after the cloning has happened - are the same. However they are two different objects, so in the future as one of the counters grows the value of the other isn't affected in any way.
Extending MyDate

In this assignment we will extend the class MyDate, that was developed in chapter 24.7. The code of the class:

public class MyDate {
    private int day;
    private int month;
    private int year;

    public MyDate(int day, int month, int year) {
        this.day = day;
        this.month = month;
        this.year = year;
    }

    public String toString() {
        return this.day + "." + this.month + "." + this.year;
    }

    public boolean earlier(MyDate compared) {
        // first we'll compare years
        if ( this.year < compared.year ) {
            return true;
        }

        // if the years are the same, we'll compare the months
        if ( this.year == compared.year && this.month < compared.month ) {
            return true;
        }

        // years and months the same, we'll compare the days
        if ( this.year == compared.year && this.month == compared.month &&
                this.day < compared.day ) {
            return true;
        }

        return false;
    }
}
  

Next day

Add to the class MyDate the method public void advance() that advances the date by one. Note: In this assignment we assume that all the months have 30 days!
Advancing many days

Add also overloaded version public void advance(int numberOfDays). This method should advance the day by the number given as parameter. Implement this method so that it calls the method advance() that was defined in the previous part of the assignment, e.g. the call advance(5) should call advance() 5 times. Again assume that all the months have 30 days!
Creation of a new date

Add to the class MyDate the method MyDate afterNumberOfDays(int days), that returns a new MyDate-object that has the date which equals the date of the object for which the method was called advance by the parameter of the method days. Again assume that all the months have 30 days!

Note that the object for which this method is called should not change!

Since the method creates a new object, the skeleton is of the form:

public MyDate afterNumberOfDays(int days){
    MyDate newMyDate = new MyDate( ... );

    // some code here

    return newMyDate;
}
  

The following code

public static void main(String[] args) {
    MyDate day = new MyDate(25, 2, 2011);
    MyDate newDate = day.afterNumberOfDays(7);
    for (int i = 1; i <= 7; ++i) {
        System.out.println("Friday after  " + i + " weeks is " + newDate);
        newDate = newDate.afterNumberOfDays(7);
    }
    System.out.println("This week's Friday is " + day);
    System.out.println("The date 790 days from this week's Friday is  " + day.afterNumberOfDays(790));
}
  

should print:

Friday after  1 weeks is 2.3.2011
Friday after  2 weeks is 9.3.2011
Friday after  3 weeks is 16.3.2011
Friday after  4 weeks is 23.3.2011
Friday after  5 weeks is 30.3.2011
Friday after  6 weeks is 7.4.2011
Friday after  7 weeks is 14.4.2011
This week's Friday is 25.2.2011
The date 790 days from this week's Friday is  5.5.2013
  

More assignments

All the new theory for this week has already been covered. However, since this week's topics are quite challenging, we will practise our routine with a couple of more exercises.
Difference of two dates

In this assignment we'll further extend the class MyDate. This assignment does not depend on the previous one, so the project contains the MyDate class that does not have the extensions of the previous assignment.
Difference in years, first version

Add to the class MyDate the method public int differenceInYears(MyDate comparedDate), that calculates the difference in years of the object for which the method is called and the object given as parameters.

Note the following

    the first vesion of the method is not very precise, it only calculates the difference of the years and does not take into account the day and month of the dates
    The method needs to work only in the case where the date given as parameter is before the date for which the method is called

With the code

public class Main {
    public static void main(String[] args) {
        MyDate first = new MyDate(24, 12, 2009);
        MyDate second = new MyDate(1, 1, 2011);
        MyDate third = new MyDate(25, 12, 2010);

        System.out.println( second + " and " + first + " difference in years: " + second.differenceInYears(first) );

        System.out.println( third + " and " + first + " difference in years: " + third.differenceInYears(first) );

        System.out.println( second + " and " + third + " difference in years: " + second.differenceInYears(third) );
    }
}
  

the output should be:

1.1.2011 and 24.12.2009 difference in years: 2     // since 2011-2009 = 2
25.12.2010 and 24.12.2009 difference in years: 1   // since 2010-2009 = 1
1.1.2011 and 25.12.2010 difference in years: 1     // since 2011-2010 = 1
  

More accuracy

Calculation of the previous version was not very exact, e.g. the difference of dates 1.1.2011 and 25.12.2010 was claimed to be one year. Modify the method so that it can calculate the difference properly. Only the full years in difference count. So if the difference of two dates would be 1 year and 364 days, only the full years are counted and the result is thus one.

The method still needs to work only in the case where the date given as parameter is before the date for which the method is called

The output for the previous example is now:

1.1.2011 and 24.12.2009 difference in years: 1
25.12.2010 and 24.12.2009 difference in years: 1
1.1.2011 and 25.12.2010 difference in years: 0
  

And the final version

Modify the method so that it works no matter which date is later, the one for which the method is called or the parameter. Example code:

public class Main {
    public static void main(String[] args) {
        MyDate first = new MyDate(24, 12, 2009);
        MyDate second = new MyDate(1, 1, 2011);
        MyDate third = new MyDate(25, 12, 2010);

        System.out.println( first + " and " + second + " difference in years: " + second.differenceInYears(first) );
        System.out.println( second + " and " + first + " difference in years: " + first.differenceInYears(second) );
        System.out.println( first + " and " + third + " difference in years: " + third.differenceInYears(first) );
        System.out.println( third + " and " + first + " difference in years: " + first.differenceInYears(third) );
        System.out.println( third + " and " + second + " difference in years: " + second.differenceInYears(third) );
        System.out.println( second + " and " + third + " difference in years: " + third.differenceInYears(second) );
    }
}
  

and the output

24.12.2009 and 1.1.2011 difference in years: 1
1.1.2011 and 24.12.2009 difference in years: 1
24.12.2009 and 25.12.2010 difference in years: 1
25.12.2010 and 24.12.2009 difference in years: 1
1.1.2011 and 25.12.2010 difference in years: 0
25.12.2010 and 1.1.2011 difference in years: 0
  

Person extended
Calculating the age based on the birthday

In chapter 24.9. Person was extended by adding to it a birthday represented as a MyDate object. It was noticed that after the addition the instance variable age has no role since the age could easily be calculated based on the current date and the birthday.

Now implement the method age that calucates and returns the age of the person.

Note: in the previous assignment we added the class MyDate method public int differenceInYears(MyDate compared). Copy the method here since it eases this assignment considerably.

import java.util.Calendar;

public class Person {
    private String name;
    private MyDate birthday;

    public Person(String name, int pp, int kk, int vv) {
        this.name = name;
        this.birthday = new MyDate(pp, kk, vv);
    }

    public int age() {
        // calculate the age based on the birthday and the current day
        // you get the current day as follows:
        // Calendar.getInstance().get(Calendar.DATE);
        // Calendar.getInstance().get(Calendar.MONTH) + 1; // January is 0 so we add one
        // Calendar.getInstance().get(Calendar.YEAR);
    }

    public String getName() {
        return this.name;
    }

    public String toString() {
        return this.name +", born "+ this.birthday;
    }
}
  

You can use the following program to test your method. Add also yourself to the program and ensure that your age is calculated correctly.

public class Main {
    public static void main(String[] args) {
        Person pekka = new Person("Pekka", 15, 2, 1993);
        Person steve = new Person("Thomas", 1, 3, 1955);

        System.out.println( steve.getName() + " age " + steve.age() + " years");
        System.out.println( pekka.getName() + " age " + pekka.age() + " years");
    }
}
  

Output:

Thomas age 59 years
Pekka age 21 years
  

Comparing ages based on birthdate

Add to the class Person the method boolean olderThan(Person compared) which compares the ages of the object for which the method is called and the object given as parameter. The method returns true if the object itself is older than the parameter.

public class Person {
    // ...

    public boolean olderThan(Person compared) {
       // compare the ages based on birthdate
    }
}
  

Test the method with the code:

public class Main {
    public static void main(String[] args) {
        Person pekka = new Person("Pekka", 15, 2, 1983);
        Person martin = new Person("Martin", 1, 3, 1983);

        System.out.println( martin.getName() + " is older than " +  pekka.getName() + ": "+ martin.olderThan(pekka) );
        System.out.println( pekka.getName() + " is older than " +  martin.getName() + ": "+ pekka.olderThan(martin) );
    }
}
  

The output should be:

Martin is older than Pekka: false
Pekka is older than Martin: true
  

New constructors

Add to the class Person two new constructors:

    public Person(String name, MyDate birthday) constructor sets the given MyDate-object to be the birthday of the person
    public Person(String name) constructor sets the current date (i.e., the date when the program is run) to be the birthday of the person

Example program:

public class Main {
    public static void main(String[] args) {
        Person pekka = new Person("Pekka", new MyDate(15, 2, 1983));
        Person steve = new Person("Steve");

        System.out.println( pekka );
        System.out.println( steve );
    }
}
  

Output:

Pekka, born 15.2.1983
Steve, born 9.2.2012
  

Note: The last line depends on the day when the code is executed!

-------------------------------------------------------------------------------------------------------------------------------


A quick recap

Let us start week 6 with two assignments that use the most important topics of week 5. You might want to read chapter 23.10 before assignment 94 and chapters 23.6 and 23.12 before assignment 95.
PhoneBook

In this assignment we are implementing a simple phone book.
Person

Start by programing the class Person which works as follows:

public static void main(String[] args) {
    Person pekka = new Person("Pekka Mikkola", "040-123123");

    System.out.println(pekka.getName());
    System.out.println(pekka.getNumber());

    System.out.println(pekka);
    pekka.changeNumber("050-333444");
    System.out.println(pekka);
}
  

The output is:

Pekka Mikkola
040-123123
Pekka Mikkola  number: 040-123123
Pekka Mikkola  number: 050-333444
  

So you have to implement the following class:

    the method public String toString(), which returns the string representation formulated as the above example shows
    constructor that sets the person name and phone number
    public String getName(), that returns the name
    public String getNumber(), that returns the phone number
    the method public void changeNumber(String newNumber), that can be used to change the phone number of the person

Adding persons to Phonebook

Program the class Phonebook that stores Person-objects using an ArrayList. At this stage you'll need the following methods:

    public void add(String name, String number) creates a Person-object and adds it to the ArrayList inside the Phonebook
    public void printAll(), prints all the persons inside the Phonebook

With the code:

public static void main(String[] args) {
    Phonebook phonebook = new Phonebook();

    phonebook.add("Pekka Mikkola", "040-123123");
    phonebook.add("Edsger Dijkstra", "045-456123");
    phonebook.add("Donald Knuth", "050-222333");

    phonebook.printAll();
}
  

the output should be:

Pekka Mikkola  number: 040-123123
Edsger Dijkstra  number: 045-456123
Donald Knuth  number: 050-222333
  

Searching for numbers from the phonebooks

Extend the class Phonebook with the method public String searchNumber(String name), that returns the phone number corresponding to the given name. If the sought person is not known the string "number not known" is returned.

Example code:

public static void main(String[] args) {
    Phonebook phonebook = new Phonebook();
    phonebook.add("Pekka Mikkola", "040-123123");
    phonebook.add("Edsger Dijkstra", "045-456123");
    phonebook.add("Donald Knuth", "050-222333");

    String number = phonebook.searchNumber("Pekka Mikkola");
    System.out.println( number );

    number = phonebook.searchNumber("Martti Tienari");
    System.out.println( number );
}
  

output:

040-123123
number not known
  

Money

In a previous assignment we stored the balance of a LyyraCard using a double variable. In reality money should not be represented as a double since the double arithmetics is not accurate. A better idea would be to implement a class that represents money. We'll start with the following class skeleton:

public class Money {

    private final int euros;
    private final int cents;

    public Money(int euros, int cents) {

        if (cents > 99) {
            euros += cents / 100;
            cents %= 100;
        }

        this.euros = euros;
        this.cents = cents;
    }

    public int euros(){
        return euros;
    }

    public int cents(){
        return cents;
    }

    public String toString() {
        String zero = "";
        if (cents <= 10) {
            zero = "0";
        }

        return euros + "." + zero + cents + "e";
    }
}
  

Notice that the instance variables euros and cents have been defined as final meaning that once the variables have been set, the value of those can not be changed. An object value of which can not be changed is said to be immutable. If we need to e.g. calculate the sum of two money objects, we need to create a new money object that represents the sum of the originals.

In the following we'll create three methods that are needed in operating with money.
Plus

Let us start by implementing the method public Money plus(Money added), that returns a new Money object that has a value equal to the sum of the object for which the method was called and the object given as parameter.

Examples of the method usage:

Money a = new Money(10,0);
Money b = new Money(5,0);

Money c = a.plus(b);

System.out.println(a);  // 10.00e
System.out.println(b);  // 5.00e
System.out.println(c);  // 15.00e

a = a.plus(c);          // NOTE: new Money-object is created and reference to that
                        //           is assigned to variable a.
                        //       The Money object 10.00e that variable a used to hold
                        //           is not referenced anymore

System.out.println(a);  // 25.00e
System.out.println(b);  // 5.00e
System.out.println(c);  // 15.00e
  

less

Create the method public boolean less(Money compared), that returns true if the object for which the method was called is less valuable than the object given as parameter.

Money a = new Money(10,0);
Money b = new Money(3,0);
Money c = new Money(5,0);

System.out.println(a.less(b));  // false
System.out.println(b.less(c));  // true

  

Minus

And finally create the method public Money minus(Money decremented), that returns a new Money object that has a value equal to the object for which the method was called minus the object given as parameter. If the value would be negative, the resulting Money object should have the value 0.

Examples of the method usage:

Money a = new Money(10,0);
Money b = new Money(3,50);

Money c = a.minus(b);

System.out.println(a);  // 10.00e
System.out.println(b);  // 3.50e
System.out.println(c);  // 6.50e

c = c.minus(a);         // NOTE: new Money-object is created and reference to that is assigned to variable c
                        //       the Money object 6.50e that variable c used to hold, is not referenced anymore

System.out.println(a);  // 10.00e
System.out.println(b);  // 3.50e
System.out.println(c);  // 0.00e
  

Character strings are immutable

The String objects of Java, as with the Money class objects, are unchangeable, immutable. If for example a new object is concatenated to the end of a character string with the + operator, the original character string doesn't become longer, but a new character string object is born:

String characterString = "test";
characterString + "tail";

System.out.println( characterString );  // test

We see that the character string cannot be changed, but we can add the value of the new character string - that was born from concatenation - to the old variable:

String characterString = "test";
characterString = characterString + "tail";   // or characterString += "tail";

System.out.println( characterString );  // testtail

Now the variable characterString refers to a new character string object, which was created by combining the previous character string value the variable referred to ("test") with the "tail" character string. Nothing refers to the "test" character string object anymore.
Array

During the course, we've used ArrayLists numerous times to store different kinds of objects. ArrayList is easy to use because it offers a lot of ready-made tools that make the programmer's life a little easier: automatic growing of a list, thanks to the list which doesn't run out of space (unless of course the list grows so large that it makes the program take up all the memory that is reserved for it), for example.

Array is an object that can be understood as a series of pigeonholes for values. The length or size of an array is the number of spots in that array - the number of items you can put in the array. The values of an array are called cells of the array. Unlike with ArrayLists, the size of the array (the amount of cells in an array) cannot be changed, growing an array always requires creating a new array and copying the cells of the old array to the new one.

An array can be created in two ways. Let's take a look at the way in which we give content to the array at creation. An array of the integer type that consists of 3 cells is defined as follows:

int[] numbers = {100, 1, 42};

The type of the Array object is denoted asint[], which stands for an array, the cells of which are of the type int. In the example the name of the array-object is numbers and it holds 3 number values {100, 1, 42}. The array is formatted with a block, in which the values to be inserted into the array are separated by commas.

The values of the array can be of any variable type that we've seen earlier. Below we've first introduced an array containing character strings and then an array containing floating numbers.

String[] characterStringArray = {"Matti P.", "Matti V."};
double[] floatingNumberArray = {1.20, 3.14, 100.0, 0.6666666667};

The cells of the array are referred to with indexes that are integers. The index tells the position of the cell in the array. The first item in an array is in position 0, the next one in position 1, and so forth. When inspecting a certain value of an array, the index is given after the name of the array object in brackets.

// index           0   1    2    3   4   5     6     7
int[] numbers = {100,  1,  42,  23,  1,  1, 3200, 3201};

System.out.println(numbers[0]);    // prints the number in the array's index 0: the number 100
System.out.println(numbers[2]);    // prints the number in the array's index 2, the number 42

The size (length) of the array above is 8.

You'll probably notice that the get-method of ArrayList works pretty much the same as getting from a certain index of an array. Only the notation - the syntax - is different when dealing with arrays.

Setting an individual value to a certain position in an array happens the same way as with regular variables, only with arrays the index also has to be mentioned. The index is mentioned inside brackets.

int[] numbers = {100,1,42};

numbers[0] = 1;    // setting value 1 to index 0
numbers[1] = 101;  // setting value 101 to index 1

// the numbers array now looks like {1,101,42}

If an index points past an array, that is, to a cell that doesn't exist, we will get an error: ArrayIndexOutOfBoundsException, which means that the index that we pointed at doesn't exist. So we cannot refer to a cell that is past the array - to an index that is smaller than 0, or larger or equals the size of the array.

We'll notice that the array clearly is related to ArrayList. Arrays, as with lists, have their cells in a certain order!
Iteration of an array

The size of an array object can be found out by typing array.length into the code, notice that you don't use parentheses with this one. array.length() does not work!

Iterating through the cells of an array is easy to implement with the help of the while-command:

int[] numbers = {1, 8, 10, 3, 5};

int i = 0;
while (i < numbers.length ) {
    System.out.println(numbers[i]);
    i++;
}

With the help of variable i we go through the indexes 0, 1, 2, 3, and 4, and print the value of the variable in each cell. First numbers[0] gets printed, then numbers[1] and so forth. The variable i stops getting increased when the array has been iterated through, that is when i's value is equal to the length of the array.

When iterating through an array it isn't always necessary to list the indexes of it, the only interesting thing is the values of the array. In this case we can use the for-each-structure - that we became familiar with earlier - to go through the values. Now only the name of a variable is given in the frame of the loop, to which each of the values of the array are set one after the other. The name of the array is separated with a colon.

int[] numbers = {1,8,10,3,5};

for (int number : numbers) {
    System.out.println(number);
}

String[] names = {"Juhana L.", "Matti P.", "Matti L.", "Pekka M."};

for (String name : names) {
    System.out.println(name);
}

Notice: when using a for-each-type of loop you cannot set values to the cells of the array! With the format of the for-sentence we inspect next that can be done too.
Another form of the for command

So far when doing loops, we've used while and the for-each form of the for sentence. Another form of the for-loop exists, which is handy especially when handling arrays. In the following we print the numbers 0, 1 and 2 with a for loop:

for (int i = 0; i < 3; i++ ) {
    System.out.println(i);
}

The for in the example works exactly as the while below:

int i = 0;  // formatting the variable that will be used in the loop
while ( i < 3 ) {  // condition
    System.out.println(i);
    i++;   // updating the variable that is used in the loop
}

a for command, as shown in for (int i = 0; i < 3; i++ ) above, has three parts to it: formatting the loop variables; condition; updating the loop variables:

    In the first part, the variables that are used in the loop are formatted. In the example above we formatted the variable i with int i=0. The first part is run only once, at the beginning of a for run.
    In the second part the condition is defined, which defines how long the code is run in the code block that is related to the for loop. In our example the condition was i < 3. The validity of the condition is checked before each round of the loop. The condition works exactly the same as the a condition of a while loop works.
    The third part, which in our example is i++ , is always run once at the end of each round of the loop.

Compared to while, for is a slightly clearer way of implementing loops of whose amount of runs is based on, for example, growing a counter. When going through an array the case is usually exactly this. In the following we print the contents of the numbers array with for:

int[] numbers = {1, 3, 5, 9, 17, 31, 57, 105};

for(int i = 3; i < 7; i++) {
    System.out.println(numbers[i]);
}

Naturally with for you don't have to start from 0 and the iteration can be done 'from top down'. For example, the cells in indexes 6, 5, 4, and 3 can be printed like this:

int[] numbers = {1, 3, 5, 9, 17, 31, 57, 105};

for(int i = 6; i>2 ; i--) {
    System.out.println(numbers[i]);
}

For and array length

Going through all cells of an array with for happens like this:

int[] numbers = {1, 8, 10, 3, 5};

for (int i = 0; i < numbers.length; i++ ) {
    System.out.println(numbers[i]);
}

Notice, that in the condition i < numbers.length we compare the value of the loop variable to the length we get from the array. The condition should not in any case be "hardcoded" as, for example, i < 5 because often the length of the array can't be known for sure beforehand.
Array as a parameter

Arrays can be used - just as any other objects - as a parameters to a method. Notice that, as with all objects, the method gets a reference to an array, so all changes done to the content of the array in the method also show up in the main program.

public static void listCells(int[] integerArray) {

    System.out.println("the cells of the array are: ");
    for( int number : integerArray) {
        System.out.print(number + " ");
    }

    System.out.println("");
}

public static void  main(String[] args) {
    int[] numbers = { 1, 2, 3, 4, 5 };
    listCells(numbers);
}

As we already know, the name of the parameter within a method can be freely chosen. The name does not need to be the same as in the one used in calling it. Above, the array is called integerArray within the method and the caller of the method knows the array as numbers.
Sum of the array

Implement the method public static sum(int[] array), which returns the sum of the numbers in the array given as parameter.

Program skeleton:

public class Main {
    public static void main(String[] args) {
        int[] array = {5, 1, 3, 4, 2};
        System.out.println(sum(array));
    }

    public static int sum(int[] array) {
        // write code here
        return 0;
    }
}
  

The output should be:

15
  

NOTE: in this and some of the following assignments methods are static as the they used to be in the assignments for weeks 2 and 3. The reason for this is that the methods are not instance methods, i.e. not operating with instance variables of objects, instead they are working at "class level" and operating just with the values and objects given as parameter. In chapter 31 we'll elaborate more on the question whether a method should be static or not.
Elegant printing of an array

Implement the method public static int printElegantly(int[] array), which prints the numbers in the array on the same row. In the printout all the numbers should be separated with comma and whitespace and there should not be a comma trailing the last number.

Program skeleton:

public class Main {
    public static void main(String[] args) {
        int[] array = {5, 1, 3, 4, 2};
        printElegantly(array);
    }

    public static void printElegantly(int[] array) {
        // write code here
    }
}
  

The output should be:

5, 1, 3, 4, 2
  

Creating a new array

If the size of the array isn't always the same, that is, if its size depends on user input for example, the previously introduced way of creating arrays will not do. It is also possible to create a table so that its size is defined with the help of a variable:

int cells = 99;
int[] array = new int[cells];

Above we create an array of the type int, that has 99 cells. With this alternative way creation of an array happens just like with any other object; with the command new. Following the new is the type of the array and in the brackets is the size of the array.

int cells = 99;
int[] array = new int[cells]; //creating an array of the size of the value in the 'cells' variable

if(array.length == cells) {
    System.out.println("The length of the array is " + cells);
} else {
    System.out.println("Something unreal happened. The length of the array is something else than " + cells);
}

In the following example there is a program that prompts for the user the amount of values and subsequently the values. After this the program prints the values in the same order again. The values given by the user are stored in the array.

System.out.print("How many values? ");
int amountOfValues = Integer.parseInt(reader.nextLine());

int[] values = new int[amountOfValues];

System.out.println("Enter values:");
for(int i = 0; i < amountOfValues; i++) {
    values[i] = Integer.parseInt(reader.nextLine());
}

System.out.println("Values again:");
for(int i = 0; i < amountOfValues; i++) {
    System.out.println(values[i]);
}

A run of the program could look something like this:

How many values? 4
Enter values:
4
8
2
1
Values again:
4
2
8
1

An array as the return value

Since methods can return objects, they can also return arrays. This particular method that returns an array looks like this -- notice that arrays might as well contain objects.

public static String[] giveStringTable() {
    String[] tchrs = new String[3];

    tchrs[0] = "Bonus";
    tchrs[1] = "Ihq";
    tchrs[2] = "Lennon";

    return tchrs;
}

public static void main(String[] args){
    String[] teachers = giveStringTable();

    for ( String teacher : teachers)
        System.out.println( teacher );
}

Reversing and copying of an array
Copy

Implement the method public static int[] copy(int[] array) that creates a copy of the parameter. Tip: since you are supposed to create a copy of the parameter, the method should create a new array where the contents of the parameter is copied.

In the following an example of the usage (note how code uses a handy helper method to print arrays):

public static void main(String[] args) {
    int[] original = {1, 2, 3, 4};
    int[] copied = copy(original);

    // change the copied
    copied[0] = 99;

    // print both
    System.out.println( "original: " + Arrays.toString(original));
    System.out.println( "copied: " + Arrays.toString(copied));
}
  

As seen in the output, the change made to the copy does not affect the original:

original: [1, 2, 3, 4]
copied: [99, 2, 3, 4]
  

Reverse copy

Implement the method public static int[] reverseCopy(int[] array) that creates an array which contains the elements of the parameter but in reversed order. The parameter array must remain the same.

E.g. if the parameter contains values 5, 6, 7 the method returns a new array that contains the values 7, 6, 5.

In the following an example of the usage:

public static void main(String[] args) {
    int[] original = {1, 2, 3, 4};
    int[] reverse = reverseCopy(original);

    // print both
    System.out.println( "original: " +Arrays.toString(original));
    System.out.println( "reversed: " +Arrays.toString(reverse));
}
  

The output should reveal that the parameter remains intact:

original: [1, 2, 3, 4]
reversed: [4, 3, 2, 1]
  

About blocks and nested loops

A piece of code that begins with a curly bracket { and ends with a curly bracket } is called a block. As we've already seen, blocks are used - among other things - to denote the code of conditional and loop sentences. An important feature of a block is that variables defined within it only exist within it..

In the following example we define the string variable stringDefinedWithinBlock within the block of a conditional sentence, which therefor will only exist within the block. The variable introduced within the block cannot be printed outside of it!

int number = 5;

if( number == 5 ){
    String stringDefinedWithinBlock = "Yeah!";
}

System.out.println(stringDefinedWithinBlock); // does not work!

However, you can use and manipulate variables defined outside of the block in the block.

int number = 5;

if( number == 5 ) {
    number = 6;
}

System.out.println(number); // prints 6

You can have any kind of code within a block. For example, a for loop can have another for loop within it or say, a while loop. Let's inspect the following program:

for(int i = 0; i < 3; i++) {
   System.out.print(i + ": ");

   for(int j = 0; j < 3; j++) {
      System.out.print(j + " ");
   }

   System.out.println();
}

The program prints the following:

0: 0 1 2
1: 0 1 2
2: 0 1 2

So what happens in the program? If we only think about the outer for loop, its functionality is easy to understand:

for(int i = 0; i < 3; i++) {
   System.out.print(i + ": ");

   // the inner for-loop

   System.out.println();
}

So first i=0 prints 0: and a carriage return. After this i grows and 1 is printed and so forth, so the outer for makes this happen:

0:
1:
2:

The inner for loop is also easy to understand separately. It prints out 0 1 2. When we combine these two, we'll notice that the inner for loop carries out its print just before the outer for loop's carriage return.
variables defined outside of a for loop as its condition

Let's inspect the following alteration to the previous example:

for(int i = 0; i < 3; i++) {
    System.out.print(i + ": ");

    for(int j = 0; j <= i; j++) {
        System.out.print(j + " ");
    }

    System.out.println();
}

The amount of runs the inner for loop does now depends on the value of the variable i of the outer loop. So when i=0 the inner loop prints 0, when i=1 the inner loop prints 0 1. The entire output of the program is as follows:

0: 0
1: 0 1
2: 0 1 2

The following program prints out the multiplication tables of the numbers 1 .. 10.

for(int i = 1; i <= 10; i++) {

    for(int j = 1; j <= 10; j++) {
        System.out.print(i * j + " ");
    }

    System.out.println();
}

The output looks like this:

1 2 3 4 5 6 7 8 9 10
2 4 6 8 10 12 14 16 18 20
3 6 9 12 15 18 21 24 27 30
4 8 12 16 20 24 28 32 36 40
5 10 15 20 25 30 35 40 45 50
6 12 18 24 30 36 42 48 54 60
7 14 21 28 35 42 49 56 63 70
8 16 24 32 40 48 56 64 72 80
9 18 27 36 45 54 63 72 81 90
10 20 30 40 50 60 70 80 90 100

The topmost row has the multiplication table of 1. At the beginning i=1 and the inner loop's variable j gets the values 1...10. For each i, j value pair their product is printed. So at the beginning i=1, j=1, then i=1, j=2, ..., i=1, j=10 next i=2, j=1, and so forth.

Of course the multiplication table program can be cut in to smaller pieces, too. We can define the methods public void printMultiplicationTableRow(int multiplier, int howManyTimes) and public void printMultiplicationTable(int upTo), in this case the structure of our program could be as follows:

public class MultiplicationTable {

    public void print(int upTo) {
        for(int i = 1; i <= upTo; i++) {
            printMultiplicationTableRow(i, upTo);

            System.out.println();
        }
    }

    public void printMultiplicationTableRow(int multiplier, int howManyTimes) {
        for(int i = 1; j <= howManyTimes; i++) {
            System.out.print(i * multiplier + " ");
        }
    }
}

Now calling new MultiplicationTable().print(5); prints the tables below.

1 2 3 4 5
2 4 6 8 10
3 6 9 12 15
4 8 12 16 20
5 10 15 20 25

Array to stars

Implement the method public static printArrayAsStars(int[] array), which prints a line with stars for each number in the array. The line length is determined by the number.

The program skeleton:

public class Main {
    public static void main(String[] args) {
        int[] array = {5, 1, 3, 4, 2};
        printArrayAsStars(array);
    }

    public static void printArrayAsStars(int[] array) {
        // code here
    }
}
  

The above example should cause the following output:

*****
*
***
****
**
  

As seen the first line has 5 stars and the reason for that is that is that the first element of the array is 5. The next line has one star since the second element of the array is 1, etc.
Night sky

Let us implement a program that prints the Night sky. The sky has a star density. If the density is e.g. 0.1, roughly 10% of the sky is covered with stars.

Stars print out as *-characters. Below an example that demonstrates how the NightSky could be used when all the steps of the assignment are done.

NightSky NightSky = new NightSky(0.1, 40, 10);
NightSky.print();
System.out.println("Number of stars: " + NightSky.starsInLastPrint());
System.out.println("");

NightSky = new NightSky(0.2, 15, 6);
NightSky.print();
System.out.println("Number of stars: " + NightSky.starsInLastPrint());
  

        *     *                  *
    *             * *         *      **
                                     *
        *       *      *         *  *
 *     *                     *
*            * *                   *
*  * *           *          * *  **
                            *  *
          *               *
     *                             *
Number of stars: 36

 * * *     *
     * *   *
*     *
   *  *       *
*       *   * *
* ** **     *
Number of stars: 22

  

Note! in the assignment use the for-clause. Despite that the previous chapter described nested loops, in this assignment we "hide" the nested loop within a method.
Class NightSky and a star line

Create the class NightSky, that has three object variables: density (double), width (int), and height (int). The class should have 3 constructors:

    public NightSky(double density) creates a NightSky object with the given star density. Width gets the value 20 and height the value 10.
    public NightSky(int width, int height) creates a NightSky object with the given width and height. Density gets the value 0.1.
    public NightSky(double density, int width, int height) creates a NightSky-object with the given density, width and height

Add to the class NightSky the method printLine, that prints one line of starts. The line length is determined by the value of the instance variable width and the instance variable density determines the star probability. For each printed character you should use a Random object to decide if it prints out as a white space or a star. The method nextDouble will probably be of use now.

In the following example:

NightSky NightSky = new NightSky(0.1, 40, 10);
NightSky.printLine();
  

            *  *                  *
  

Printing the night sky

Add the class NightSky the method print, that prints the night sky of the given size. Use the method printLine to print each separate line of the night sky. An example in the following:

NightSky NightSky = new NightSky(8, 4);
NightSky.print();
  

    *

  *
    *
  

Counting the number of stars

Add the class NightSky an instance variable starsInLastPrint (int) and the method starsInLastPrint(), that returns the number of stars printed in the previous night sky. Example in the below:

NightSky NightSky = new NightSky(8, 4);
NightSky.print();
System.out.println("Number of stars: " + NightSky.starsInLastPrint());
System.out.println("");

NightSky.print();
System.out.println("Number of stars: " + NightSky.starsInLastPrint());
  


 *

Number of stars: 1

 *
      *
*

Number of stars: 3
  

To static or not to static?

When we started using objects, the material advised to leave out the keyword 'static' when defining their methods. However, up until week 3 all of the methods included that keyword. So what is it all about?

The following example has a method resetArray, that works as its name implies; it sets all of the cells of an array that it receives as a parameter to 0.

public class Program {

    public static void resetArray(int[] table) {
        for ( int i=0; i < table.length; i++ )
            table[i] = 0;
    }

    public static void main(String[] args) {
        int[] values = { 1, 2, 3, 4, 5 };

        for ( int number : values ) {
            System.out.print( number + " " );  // prints 1, 2, 3, 4, 5
        }

        System.out.println();

        resetArray(values);

        for ( int number : values ) {
            System.out.print( number + " " );  // prints 0, 0, 0, 0, 0
        }
    }
}

We notice that the method definition now has the keyword static. The reason for that is that the method does not operate on any object, instead it is a class method or in other words static methods. In contrast to instance methods, static methods are not connected to any particular object and thus the reference this is not valid within static methods. A static method can operate only with data that is given it as parameter. The parameter of a static method can naturally be an object.

Since static methods are not connected to any object, those can not be called through the object name: objectName.methodName() but should be called as in the above example by using only the method name.

If the static method is called from a different class, the call is of the form ClassName.staticMethodName(). The below example demonstrates that:

public class Program {
    public static void main(String[] args) {
        int[] values = { 1, 2, 3, 4, 5 };

        for ( int value : values ) {
            System.out.print( value + " " );  // prints: 1, 2, 3, 4, 5
        }

        System.out.println();

        ArrayHandling.resetArray(values);

        for ( int value : values ) {
            System.out.print( value + " " );  // prints: 0, 0, 0, 0, 0
        }
    }
}

public class ArrayHandling {
    public static void resetArray(int[] array) {
        for ( int i=0; i < array.length; i++ ) {
            array[i] = 0;
        }
    }
}

The static method that has been defined within another class will now be called with ArrayHandling.resetArray(parameter);.
When static methods should be used

All object state-handling methods should be defined as normal object methods. For example, all of the methods of the Person, MyDate, Clock, Team, ... classes we defined during the previous weeks should be defined as normal object methods, not as statics.

Lets get back to the Person class yet again. In the following is a part of the class definition. All of the object variables are referred to with the this keyword because we emphasize that we are handling the object variables 'within' the said object..

public class Person {
    private String name;
    private int age;

    public Person(String name) {
        this.age = 0;
        this.name = name;
    }

    public boolean isAdult(){
        if ( this.age < 18 ) {
            return false;
        }

        return true;
    }

    public void becomeOlder() {
        this.age++;
    }

    public String getName() {
        return this.name;
    }
}

Because the methods manipulate the object, they do not need to be defined as static, or in other words "not belonging to the object". If we try to do this, the program won't work:

public class Person {
    //...

    public static void becomeOlder() {
        this.age++;
    }
}

As a result we'll get an error non-static variable age can not be referenced from static context, which means that a static method cannot handle an object method.

So when should a static method be used then? Let us inspect the Person object handling an example familiar from chapter 23:

public class Program {
    public static void main(String[] args) {
        Person pekka = new Person("Pekka");
        Person antti = new Person("Antti");
        Person juhana = new Person("Juhana");

        for ( int i=0; i < 30; i++ ) {
            pekka.becomeOlder();
            juhana.becomeOlder();
        }

        antti.becomeOlder();

        if ( antti.isAdult() ) {
            System.out.println( antti.getName() + " is an adult" );
        } else {
            System.out.println( antti.getName() + " is a minor" );
        }

        if ( pekka.isAdult() ) {
            System.out.println( pekka.getName() + " is an adult" );
        } else {
            System.out.println( pekka.getName() + " is a minor" );
        }

        if ( juhana.isAdult() ) {
            System.out.println( juhana.getName() + " is an adult" );
        } else {
            System.out.println( juhana.getName() + " is a minor" );
        }
    }
}

We'll notice that the piece of code that reports the matureness of persons is copy-pasted twice in the program. It looks really bad!

Reporting the maturity of a person is an excellent candidate for a static method. Let's rewrite the Program using that method:

public class Main {

    public static void main(String[] args) {
        Person pekka = new Person("Pekka");
        Person antti = new Person("Antti");
        Person juhana = new Person("Juhana");

        for ( int i=0; i < 30; i++ ) {
            pekka.becomeOlder();
            juhana.becomeOlder();
        }

        antti.becomeOlder();

        reportMaturity(antti);

        reportMaturity(pekka);

        reportMaturity(juhana);
    }

    private static void reportMaturity(Person person) {
        if ( person.isAdult() ) {
            System.out.println(person.getName() + " is an adult");
        } else {
            System.out.println(person.getName() + " is a minor");
        }
    }
}

The method reportMaturity is defined as static so it doesn't belong to any object, but the method receives a Person object as a parameter. The method is not defined within the Person-class since even though it handles a Person object that it receives as a parameter, it is an assistance method of the main program we just wrote. With the method we've made main more readable.
The library information system

In this assignment we are implementing a simple information system prototype for a library. The prototype will have functionality for searching books by the title, publisher or publishing year.

The main building blocks of the system are the classes Book and Library. Objects of the class Book represent the information of a single book. Object of the class Library holds a set of books and provides various ways to search for the books within the library.
Book

Let us start with the class Book. The class has instance variables title for the book title, publisher for the name of the publisher, and year for the publishing year. The title and the publisher are of the type String and the publishing year is represented as an integer.

Now implement the class Book. The class should have the constructor public Book(String title, String publisher, int year) and methods public String title(), public String publisher(), public int year() and public String toString().

Example usage:

Book cheese = new Book("Cheese Problems Solved", "Woodhead Publishing", 2007);
System.out.println(cheese.title());
System.out.println(cheese.publisher());
System.out.println(cheese.year());

System.out.println(cheese);
  

The output should be:

Cheese Problems Solved
Woodhead Publishing
2007
Cheese Problems Solved, Woodhead Publishing, 2007
  

Library

Implement the class Library, with constructor public Library() and methods public void addBook(Book newBook) and public void printBooks()

Example usage below.

Library Library = new Library();

Book cheese = new Book("Cheese Problems Solved", "Woodhead Publishing", 2007);
Library.addBook(cheese);

Book nhl = new Book("NHL Hockey", "Stanley Kupp", 1952);
Library.addBook(nhl);

Library.addBook(new Book("Battle Axes", "Tom A. Hawk", 1851));

Library.printBooks();
  

The output should be:

Cheese Problems Solved, Woodhead Publishing, 2007
NHL Hockey, Stanley Kupp, 1952
Battle Axes, Tom A. Hawk, 1851
  

Search functionality

Add to the class Library the methods public ArrayList<Book> searchByTitle(String title), public ArrayList<Book> searchByPublisher(String publisher) and public ArrayList<Book> searchByYear(int year). The methods return the list of books that match the given title, publisher or year.

Note: you are supposed to do a method that returns an ArrayList. Use the following skeleton as starting point:

public class Library {
   // ...

   public ArrayList<Book> searchByTitle(String title) {
     ArrayList<Book> found = new ArrayList<Book>();

     // iterate the list of books and add all the matching books to the list found

     return found;
   }
  

Note: when you do the search by a string (title or publisher), do not look for exact matches (with the method equals) instead use the method contains of the class String.

Example usage:

Library Library = new Library();

Library.addBook(new Book("Cheese Problems Solved", "Woodhead Publishing", 2007));
Library.addBook(new Book("The Stinky Cheese Man and Other Fairly Stupid Tales", "Penguin Group", 1992));
Library.addBook(new Book("NHL Hockey", "Stanley Kupp", 1952));
Library.addBook(new Book("Battle Axes", "Tom A. Hawk", 1851));

ArrayList<Book> result = Library.searchByTitle("Cheese");
for (Book book: result) {
    System.out.println(book);
}

System.out.println("---");
for (Book book: Library.searchByPublisher("Penguin Group  ")) {
    System.out.println(book);
}

System.out.println("---");
for (Book book: Library.searchByYear(1851)) {
    System.out.println(book);
}
  

The output should be:

Cheese Problems Solved, Woodhead Publishing, 2007
The Stinky Cheese Man and Other Fairly Stupid Tales, Penguin Group, 1992
---
---
Battle Axes, Tom A. Hawk, 1851
  

Improved search

There are some minor problems with the implemented search functionality. One particular problem is that the search differentiates upper and lower case letters. In the above example the search by title with the search term "cheese" produced an empty list as answer. The example where the search term contained extra white spaces did not give the expected answer, either. We'd like the search functionality to be case insensitive and not disturbed by the extra white spaces at the start or at the end of the search terms. We will implement a small helper library StringUtils that will then be used in the Library for the more flexible search functionality.

Implement the class StringUtils with a static method public static boolean included(String word, String searched), which checks if the string searched is contained within the string word. As described in the previous paragraph, the method should be case insensitive and should not care about trailing and ending white spaces in the string searched. If either of the strings is null, the method should return false.

Tip: The methods trim and toUpperCase() of the class String might be helpful.

When you have completed the method, use it in the search functionality of the class Library.

Use the method as follows:

if(StringUtils.included(book.title(), searchedTitle)) {
    // Book found!
}
  

The improved library with the example:

Library Library = new Library();

Library.addBook(new Book("Cheese Problems Solved", "Woodhead Publishing", 2007));
Library.addBook(new Book("The Stinky Cheese Man and Other Fairly Stupid Tales", "Penguin Group", 1992));
Library.addBook(new Book("NHL Hockey", "Stanley Kupp", 1952));
Library.addBook(new Book("Battle Axes", "Tom A. Hawk", 1851));

for (Book book: Library.searchByTitle("CHEESE")) {
    System.out.println(book);
}

System.out.println("---");
for (Book book: Library.searchByPublisher("PENGUIN  ")) {
    System.out.println(book);
}
  

should output the following:

Cheese Problems Solved, Woodhead Publishing, 2007
The Stinky Cheese Man and Other Fairly Stupid Tales, Penguin Group, 1992
---
The Stinky Cheese Man and Other Fairly Stupid Tales, Penguin Group, 1992
  

Assignments where you are free to decide how to structure the program.
Grade distribution

This assignment corresponds to three assignment points.

Note1: Your program should use only one Scanner object, i.e., it is allowed to call new Scanner only once. If you need scanner in multiple places, you can pass it as parameter:

public static void main(String[] args) {
    Scanner scanner = new Scanner(System.in);

    // ...

    doSomething(scanner);
}

public static void doSomething(Scanner scanner) {
    String riw = scanner.nextLine();
    // ...
}
  

If another object needs a scanner, you can pass it as constructor parameter and save in instance variable.

Note2: Do not save anything in static variables. The main method is executed by the tests multiple times so the use of static variables might cause problems.

The input of the program is a set of exam scores of a course. Each score is an integer. When -1 is entered, the program stops asking for further input.

Inputting the exam scores should work as follows:

Type exam scores, -1 completes:
34
41
53
36
55
27
43
40
-1
  

After the scores have been read, the program prints the grade distribution and acceptance percentage of the course in the following form:

Grade distribution:
5: **
4:
3: ***
2: *
1: *
0: *
Acceptance percentage: 87.5
  

Grade distribution is formed as follows:

    Each exam score is mapped to a grade using the same formula as in exercise 18. If the score is not within the range 0-60 it is not taken into account.
    The number of grades are printed as stars, e.g. if there are 2 scores that correspond to grade 5, the line 5: ** is printed. If there are no scores that correspond to a particular grade, as is the case with grade 4 in the above example, the printed line is 4:

All the grades besides zeros are accepted, so in the above 7 out of 8 participants were accepted. Acceptance percentage is calculated with the formula 100*accepted/allScores.
Birdwatchers database

Note1: Your program should use only one Scanner object, i.e., it is allowed to call new Scanner only once.

Note2: Do not save anything in static variables. The main method is executed by the tests multiple times so the use of static variables might cause problems.

This assignment corresponds to three assignment points.

In this assignment you are supposed to design and implement an observation database for a bird watcher. The database contains birds, each of which have a name and a Latin name, both Strings. Database also tracks how many times each bird has been observed.

The program should implement the following commands:

    Add - adds a bird
    Observation - adds an observation
    Statistics - prints all the birds
    Show - prints one bird
    Quit - terminates the program

The program should also handle the invalid inputs (see Turing below).

The following is an example how the program is supposed to work:

? Add
Name: Raven
Latin Name: Corvus Corvus
? Add
Name: Seagull
Latin Name: Dorkus Dorkus
? Observation
What was observed:? Seagull
? Observation
What was observed:? Turing
Is not a bird!
? Observation
What was observed:? Seagull
? Statistics
Seagull (Dorkus Dorkus): 2 observations
Raven (Corvus Corvus): 0 observations
? Show
What? Seagull
Seagull (Dorkus Dorkus): 2 observations
? Quit
  

Note you may structure your program freely, it is only required that the output of the program is as in the above example.
Sorting an array

We'll get back to arrays again.
Sorting an array with the ready-made tools of Java.

As we've seen, there's all kinds of useful things already in Java. For example for handling ArrayLists you can find many useful help methods in the class Collections. For arrays you can find helpful methods in the class Arrays. Sorting a table can be done with Arrays.sort(array).

Note: To be able to use the command you must have the following definition at the top of the program file:

import java.util.Arrays;

If you forget to write the import line, NetBeans will offer help with writing it. Try clicking the picture of the "bulp" that appears to the left from the line of code that is underlined with red.

The following program creates arrays and sorts the values in the array with the Arrays.sort -command.

int[] values = {-3, -111, 7, 42};
Arrays.sort(values);
for(int value: values) {
    System.out.println(value);
}

-111
-3
7
42

Implementation of a sorting algorithm

It's easy to sort an array with the ready-made tools of Java. The general knowledge of a program requires knowing at least one sorting algorithm (or in other words, a way to sort an array). Let's get familiar with the "classic" sorting algorithm, choice sorting. Let's do this with a few excercise.
Sorting

Note: in this assignment you're supposed to sort the array yourself. You can't use the help of the Arrays.sort()-method or ArrayLists!
Smallest

Implement a method smallest, which returns the smallest value in the array.

The frame of the method is as follows:

public static int smallest(int[] array) {
    // write the code here
}
  

NOTE: You can't change the array that gets passed into the method!

The following code demonstrates the functionality of the method:

int[] values = {6, 5, 8, 7, 11};
System.out.println("smallest: " + smallest(values));
  

smallest: 5
  

The index of the smallest

Implement a method indexOfTheSmallest, which returns the index of the smallest value in the array (the position of the value in the array, that is).

The frame of the method looks like this:

public static int indexOfTheSmallest(int[] array) {
    // code goes here
}
  

NOTE: You can't change the array that gets passed into the method as a parameter!

The following code demonstrates the functionality of the method:

// indexes:   0  1  2  3  4
int[] values = {6, 5, 8, 7, 11};
System.out.println("Index of the smallest: " + indexOfTheSmallest(values));
  

Index of the smallest: 1
  

The smallest value of the table is 2 and its index (its location) in the array is 1. Remember that the numbering of an array begins from 0.
Index of the smallest at the end of an array

Implement a method indexOfTheSmallestStartingFrom, which works just like the method of the previous assignment, but only takes into consideration the end of an array starting from a certain index. In addition to the array the method gets as parameter an index, from which the search for the smallest will be started.

The frame of the method is as follows:

public static int indexOfTheSmallestStartingFrom(int[] array, int index) {
    // write the code here
}
  

NOTE: You can't change the array that gets passed into the method as a parameter!

The following code demonstrates the functionality of the method:

// indexes:    0  1  2  3   4
int[] values = {-1, 6, 9, 8, 12};
System.out.println(indexOfTheSmallestStartingFrom(values, 1));
System.out.println(indexOfTheSmallestStartingFrom(values, 2));
System.out.println(indexOfTheSmallestStartingFrom(values, 4));
  

1
3
4
  

In the example, the first method call finds the index of the smallest value starting from index 1. Starting from index 1 the smallest value is 6, and its index is 1. Respectively the second method call looks for the index of the smallest value starting from index 2. In this case the smallest value is 8 and its index is 3. The last call starts from the last cell of the array, in this case there is no other cells so the smallets value is in index 4.
Swapping values

Create a method swap, to which will be passed an array and two of its indexes. The method swaps the values in the indexes around.

The frame of the method looks like this:

public static void swap(int[] array, int index1, int index2) {
    // code goes here
}
  

The following showcases the functionality of the method. In printing the array we'll use the Arrays.toString-method which formats the array into a string:

int[] values = {3, 2, 5, 4, 8};

System.out.println( Arrays.toString(values) );

swap(values, 1, 0);
System.out.println( Arrays.toString(values) );

swap(values, 0, 3);
System.out.println( Arrays.toString(values) );
  

[3, 2, 5, 4, 8]
[2, 3, 5, 4, 8]
[4, 3, 5, 2, 8]
  

Sorting

Now we've got a set of useful methods, with which we can implement a sorting algorithm known as selection sorting.

The idea of selection sorting is this:

    Move the smallest number of the array to index 0.
    Move the second smallest number to the index 1.
    Move the third smallest number to the index 2.
    and so forth

In other words:

    Inspect the array starting from index 0. Swap the value in index 0 and the smallest value in the array starting from index 0.
    Inspect the array starting from index 1. Swap the value in index 1 and the smallest value in the array starting from index 1.
    Inspect the array starting from index 2. Swap the value in index 2 and the smallest value in the array starting from index 2.
    and so forth

Implement the method sort, which is based on the idea above. The method ought to have a loop that goes through the indexes of the array. The methods smallestIndexStartingFrom and swap are surely useful. Also print the contents of the array before sorting and after each round to be able to make sure that the algorithm works correctly.

Body of the method:

public static void sort(int[] array) {
}
  

Test the functionality of the method at least with this example:

int[] values = {8, 3, 7, 9, 1, 2, 4};
sort(values);
  

The program should print the following. Notice that you're to print the content of the array after each swap!

[8, 3, 7, 9, 1, 2, 4]
[1, 3, 7, 9, 8, 2, 4]
[1, 2, 7, 9, 8, 3, 4]
[1, 2, 3, 9, 8, 7, 4]
[1, 2, 3, 4, 8, 7, 9]
[1, 2, 3, 4, 7, 8, 9]
[1, 2, 3, 4, 7, 8, 9]
  

You'll notice how the array little by little gets sorted out starting from the beginning and advances towards the end.
Searching

In addition to sorting, another very typical problem that a programmer runs into is finding a certain value in an array. Earlier, we've implemented methods that search for values in lists and arrays. In the case of arrays, values and strings can be searched for in the following way:

public static boolean isInArray(int[] array, int searchingFor) {
    for ( int value : array ) {
       if ( value == searchingFor )  {
           return true;
       }
    }

    return false;
}

public static boolean isWordInArray(String[] array, String searchingFor) {
    for ( String word: array ) {
        if ( word.equals(searchingFor) )  {
            return true;
        }
    }

    return false;
}

An implementation like this is the best we've been able to do so far. The downside of the method is that, if the array has a very large amount of values in it, the search will take a lot of time. In the worst case scenario the method goes through every single cell in the array. This means that going through an array that has 16777216 cells does 16777216 cell inspections.

On the other hand, if the values in an array are ordered by size, the search can be done in a notably faster way by applying a technique called binary search. Let's investigate the idea of binary search with this array:

// indexes   0   1   2   3    4   5    6   7   8   9  10
// values     -7  -3   3   7   11  15   17  21  24  28  30

Let's assume that we want to find the value 17. Let's utilize the information that the values of the array are in order instead of going through the array from the beginning. Let's inspect the middle cell of the array. The middle cell is 5 (the largest index 10 divided by two). The middle cell is marked with the asterisk:

                                   *
// indexes   0   1   2   3    4   5    6   7   8   9  10
// values     -7  -3   3   7   11  15   17  21  24  28  30

At the middle is the value 15, which was not the value we were looking for. We're looking for the value 17, so since the cells of the array are ordered by size, the value cannot be on the left side of the 15. So we can determine that all indexes that are smaller or equal to 5 do not have the value we are looking for.

The area where we are searching for the value we want to find can now be limited to values that are on the right side of the index 5, or in other words, in the indexes [6, 10] (6, 7, 8, 9, 10). In the following, the searched value cannot be in the part of the array which is grey:

// indexes    0   1   2   3   4    5    6     7   8   9  10
// values      -7  -3   3   7  11   15   17   21  24  28  30

Next, let's inspect the middle index of the area that we have left; the middle index of indexes 6-10. The middle index can be found by getting the sum of the smallest and largest index and dividing it by two: (6+10)/2 = 16/2 = 8. The index 8 is marked with the asterisk below.

                                                 *
// indexes    0   1   2   3   4    5    6   7   8   9  10
// values      -7  -3   3   7  11   15   17   21  24  28  30

In index 8, we have the value 24, which was not the value we were looking for. Because the values in the array are ordered by size, the value we are searching for can not, in any case, be on the right side of the value 24. We can deduce that all indexes that are larger or equal to 8 can not contain the value we are looking for. The search area gets narrowed down again, the grey areas have been dealt with:

// indexes    0   1   2   3   4    5    6   7   8   9  10
// values      -7  -3   3   7  11   15   17   21  24  28  30

The search continues. Let's inspect the middle index of the area that we have left to search, that is, the middle index of indexes 6-7. The middle index can again be found out by getting the sum of the smallest and largest index of the search area and then dividing it by two: (6+7)/2 = 6.5, which is rounded down to 6. The spot has been marked with the asterisk.

                                         *
// indexes    0   1   2   3   4    5    6    7   8   9  10
// values      -7  -3   3   7  11   15   17   21  24  28  30

In the index 6 we have the value 17, which is the same as the value we've been looking for. We can stop the search and report that the value we searched for is in the array. If the value wouldn't have been in the array - for example if the searched-for value would've been 16 - the search area would have eventually been reduced to nothing.

                                         *
// indexes    0   1   2   3   4    56   7   8   9  10
// values      -7  -3   3   7  11   1517  21  24  28  30

So for the idea of binary search to become clear to you, simulate with pen and paper how the binary search works when the array is the one below and first you're searching for value 33 and then value 1.

// indexes   0   1   2   3   4   5   6   7   8   9  10  11  12  13
// values     -5  -2   3   5   8  11  14  20  22  26  29  33  38  41

With the help of binary search we look for cells by always halving the inspected area. This enables us to search in a very efficient way. For example, an array of size 16 can be divided in half up to 4 times, so 16 -> 8 -> 4 -> 2 -> 1. On the other hand, an array that has 16777216 cells can be halved up to 24 times. This means that with binary search we only need to inspect up to 24 cells in an array that has 16777216 cells in order to find our desired cell.

The efficiency of binary search can be inspected with logarithms. A base two logarithm (log2) of the number 16777216 is 24 -- with the base two logarithm we can calculate how many times a number can be halved. Respectively the base two logarithm of the number 4294967296 (log2 4294967296) is 32. This means that searching from a sorted array of 4294967296 different values would only take up to 32 cell inspections. Efficiency is an essential part of computer science.
Guessing game

In this assignment we'll make an AI, which guesses the number the player is thinking about. The AI assumes that the number is between lowerLimit...upperLimit. The start of the game provides these limits to the method as parameters that makes the game happen. The AI asks the player questions in the format "Is your number greater than X?" and deduce the correct answer from the answers the player gives.

The AI keeps track of the search area with the help of the variables lowerLimit and upperLimit. The AI always asks if the player's number is greater than the average of these two numbers, and based on the answers the search area gets halved each time. In the end the lowerLimit and upperLimit are the same and the number the user is thinking of has been revealed.

In the following example the user chooses the number 44:

Think of a number between 1...100.
I promise you that I can guess the number you are thinking of with 7 questions.

Next I'll present you a series of questions. Answer them honestly.

Is your number greater than 50? (y/n)
n
Is your number greater than 25? (y/n)
y
Is your number greater than 38? (y/n)
y
Is your number greater than 44? (y/n)
n
Is your number greater than 41? (y/n)
y
Is your number greater than 43? (y/n)
y
The number you're thinking of is 44.
  

In the above example the possible value range is first 1...100. When the user tells the program that the number is not greater than 50 the possible range is 1...50. When the user says that the number is greater than 25, the range is 26...50. The deduction proceeds in the same fashion until the number 44 is reached.

In accordance to the principles of halving, or binary search, the possible search area is halved after each question in which case the number of required questions is small. Even between the numbers 1...100000 it shouldn't take more than 20 questions.

The program skeleton of the class GuessingGame that implements this is the following:

public class GuessingGame {

    private Scanner reader;

    public GuessingGame() {
        this.reader = new Scanner(System.in);
    }

    public void play(int lowerLimit, int upperLimit) {
        instructions(upperLimit, lowerlimit);

        // write the game logic here
    }

    // implement here the methods isGreaterThan and average

    public void instructions(int lowerLimit, int upperLimit) {
        int maxQuestions = howManyTimesHalvable(upperLimit - lowerLimit);

        System.out.println("Think of a number between " + lowerLimit + "..." + upperLimit + ".");

        System.out.println("I promise you that I can guess the number you are thinking of with " + maxQuestions + " questions.");
        System.out.println("");
        System.out.println("Next I'll present you with a series of questions. Answer them honestly.");
        System.out.println("");
    }

    // a helper method:
    public static int howManyTimesHalvable(int number) {
        // we create a base two logarithm  of the given value
        // Below we swap the base number to base two logarithms!
        return (int) (Math.log(number) / Math.log(2)) + 1;
    }
}
  

The game is started the in following manner:

GuessingGame game = new GuessingGame();

// we play two rounds
game.play(1,10);  // value to be guessed now within range 1-10
game.play(10,99);  // value to be guessed now within range 10-99
  

We'll implement this assignment in steps.
Is greater than

Implement the method public boolean isGreaterThan(int value), which presents the user with a question:

"Is your number greater than given value? (y/n)"
  

The method returns the value true if the user replies "y", otherwise false.

Test your method

GuessingGame game = new GuessingGame();

System.out.println(game.isGreaterThan(32));
  

Is your number greater than 32? (y/n)
y
true
  

Average

Implement the method public int average(int firstNumber, int secondNumber), which calculates the average of the given values. Notice that Java rounds floating numbers down automatically, in our case this is perfectly fine.

GuessingGame game = new GuessingGame();
System.out.println(game.average(3, 4));
  

3
  

GuessingGame game = new GuessingGame();
System.out.println(game.average(6, 12));
  

9
  

Guessing logic

Write the actual guessing logic in the method play of the class GuessingGame. You'll need at least one loop and a query in which you ask the user if their number is greater than the average of the lowerLimit and upperLimit. Change the upperLimit or lowerLimit depending on the user's reply.

Keep doing the loop until lowerLimit and upperLimit are the same! You can also test the game with smaller lower- and upperLimit values:

Think of a number between 1...4.
I promise you that I can guess the number you are thinking of with 2 questions.

Next I'll present you with a series of questions. Answer them honestly.

Is your number greater than 2? (y/n)
k
Is your number greater than 3? (y/n)
k
The number you're thinking of is 4.
  

Implementation of binary search

The template you get from the test automaton has a start for an implementation of binary search. The class BinarySearch holds a method public static boolean search(int[] array, int searchedValue), the job of which is to figure out, by using binary search, if the value given as a parameter is in the sorted array that is also given as parameter.

The method search does not work yet, however. Finish the method's implementation into a real binary search.

For testing, a separate main program can be found in the class Main, which has a frame like this:

import java.util.Arrays;
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        // Here you can test binary search
        int[] array = { -3, 2, 3, 4, 7, 8, 12 };
        Scanner reader = new Scanner(System.in);

        System.out.print("Values of the array: " + Arrays.toString(array));
        System.out.println();

        System.out.print("Enter searched number: ");
        String searchedValue = reader.nextLine();
        System.out.println();

        boolean result = BinarySearch.search(array, Integer.parseInt(searchedValue));

        // Print the binary search result here
    }
}
  

The execution of the program looks like this:

Values of the array: [-3, 2, 3, 4, 7, 8, 12]

Enter searcher number: 8

Value 8 is in the array
  

Values of the array: [-3, 2, 3, 4, 7, 8, 12]

Enter searcher number: 99

Value 99 is not in the array
  

About arrays and objects

If need be, any type of object can be put into an array. In the following, an example of an array into which will be put Person objects:

public static void main(String[] args) {
    Person[] persons = new Person[3];

    persons[0] = new Person("Pekka");
    persons[1] = new Person("Antti");
    persons[2] = new Person("Juhana");

    for ( int i=0; i < 30; i++ ) {
        persons[0].becomeOlder();
        persons[1].becomeOlder();
        persons[2].becomeOlder();
    }

    for ( Person person : persons ) {
        reportMaturity(person);
    }
}

First we create an array that can hold 3 Person objects. We put Pekka in slot 0, Antti in 1 and Juhana in 2. We age all by 30 years and check all of their matureness with the help of the method from the previous chapter.

The same example with ArrayLists:

public static void main(String[] args) {
    ArrayList<Person> persons = new ArrayList<Person>();

    persons.add( new Person("Pekka") );
    persons.add( new Person("Antti") );
    persons.add( new Person("Juhana") );

    for ( int i=0; i < 30; i++ ) {
        for ( Person person : persons ) {
            person.becomeOlder();
        }

        //  or persons.get(0).becomeOlder();
        //     persons.get(1).becomeOlder();
        //     ...
    }

    for ( Person person : persons ) {
        reportMaturity(person);
    }
}

In most situations it's better to use ArrayList instead of an array. However there can be cases where an array is adequate and is simpler to use.

A week always consists of seven days. It would be meaningful to form it out of exactly 7 Day objects. Since there's always 7 Day objects, an array will suit the situation very well:

public class Day {
    private String name;
    // ...
}

public class Week {
    private Day[] days;

    public Week(){
        days = new Day[7];
        days[0] = new Day("Monday");
        days[1] = new Day("Tuesday");
        // ...
    }
}

Final Words

Object-Oriented Programming with Java, Part I ends here. Congratulations for making it this far! If you want to continue learning and programming, start our second part of the course here: Object-Oriented Programming with Java, Part II

Assuming you have NetBeans and TMC already installed in your computer, in NetBeans just change the current course from TMC -> Settings to 2013-OOProgrammingWithJava-PART2 and you should be good to go!


Helsingin yliopiston tietojenkäsittelytieteen laitos 

