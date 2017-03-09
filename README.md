# Portfolio

https://github.com/karamk-immalle/Balloon


Built-in Data Types

There are a number of built-in data types in C#. The most common are:
int - integer.
float - floating point number.
double - double-precision version of float.
char - a single character.
bool - Boolean that can have only one of two values: True or False.
string - a sequence of characters.
The statements below use C# data types:

> int x = 42;

> double pi = 3.14;

> char y = 'Z';

> bool isOnline = true;

> string firstName = "David";


Displaying Output

Most applications require some input from the user and give output as a result.
To display text to the console window you use the Console.Write or Console.WriteLine methods. The difference between these two is that Console.WriteLine is followed by a line terminator, which moves the cursor to the next line after the text output. 
The program below will display Hello World! to the console window:

>static void Main(string[] args)

>{

 >  Console.WriteLine("Hello World!");
 
 > }
 
 
 We can display variable values to the console window:
 
> static void Main(string[] args)

>{

>int x = 89;

>Console.WriteLine(x);

>}

>// Outputs 89
  

To display a formatted string, use the following syntax:

>static void Main(string[] args)

>{
 
 >int x = 10;
  
 > double y = 20;
 
  > Console.WriteLine("x = {0}; y = {1}", x, y);

>}

>// Output: x = 10; y = 20


The if statement is a conditional statement that executes a block of code when a condition is true.

The general form of the if statement is:

>if (condition)

>{

>    // Execute this code when condition is true

>}


The condition can be any expression that returns true or false. 

For example:

>static void Main(string[] args)

>{

>  int x = 8;

> int y = 3;
 
>if (x > y)

>{ 

>  Console.WriteLine("x is greater than y");

>}

>}


The code above will evaluate the condition x > y. If it is true, the code inside the if block will execute.

The else Clause

An optional else clause can be specified to execute a block of code when the condition in the if statement evaluates to false.
Syntax:

>if (condition) 

>{
 
 >//statements

>}

>else 

>{

>  //statements

>}

For example:

>int mark = 85;

>if (mark < 50) 

>{

>Console.WriteLine("You failed.");

>}

>else 

>{
 
 >Console.WriteLine("You passed.");

>}

>// Outputs "You passed." 

You can also include, or nest, if statements within another if statement.
For example:

>int mark = 100;

>if (mark >= 50) {
 
 >Console.WriteLine("You passed.");
  
  >if (mark == 100) {
   
   >Console.WriteLine("Perfect!");
  
  >}

>}

>else {
 
 >Console.WriteLine("You failed.");

>}

>Outputs
"You passed.
Perfect!"

The if-else if Statement

The if-else if statement can be used to decide among three or more actions.
For example:

>int x = 33;

>if (x == 8) {
 
 >Console.WriteLine("Value of x is 8");

>}

>else if (x == 18) {

>Console.WriteLine("Value of x is 18");

>}

>else if (x == 33) {
 
 >Console.WriteLine("Value of x is 33");

>}

>else {
 
 >Console.WriteLine("No match");

>}

>//Outputs "Value of x is 33"


What is a Method?


A method is a group of statements that perform a particular task.
In addition to the C# built-in methods, you may also define your own. 

Methods have many advantages, including:
- Reusable code.
- Easy to test.
- Modifications to a method do not affect the calling program.
- One method can accept many different inputs.

Declaring Methods

To use a method, you need to declare the method and then call it.
Each method declaration includes:
- the return type
- the method name
- an optional list of parameters.


For example, the following method has an int parameter and returns the number squared:

>int Sqr(int x)

>{
 
 >int result = x*x;
  
  >return result;

>}

The return type of a method is declared before its name. In the example above, the return type is int, which indicates that the method returns an integer value. When a method returns a value, it must include a return statement. Methods that return a value are often used in assignment statements.
Occasionally, a method performs the desired operations without returning a value. Such methods have a return type void. In this case, the method cannot be called as part of an assignment statement.


Calling Methods

Parameters are optional; that is, you can have a method with no parameters.
As an example, let's define a method that does not return a value, and just prints a line of text to the screen.

>static void SayHi()

>{

> Console.WriteLine("Hello");

>}

Our method, entitled SayHi, returns void, and has no parameters. 
To execute a method, you simply call the method by using the name and any required arguments in a statement.

>static void SayHi()

>{

>  Console.WriteLine("Hello");

>}

>static void Main(string[] args)

>{

>  SayHi();

>}

>//Outputs "Hello"

>You can call the same method multiple times:

>static void SayHi()

>{

>  Console.WriteLine("Hello");

>}

>static void Main(string[] args)

>{
  
  >SayHi();
  
  >SayHi();
  
  >SayHi();

>}
 
 Outputs:
Hello
Hello
Hello 

