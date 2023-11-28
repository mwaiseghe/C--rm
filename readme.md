# C-Sharp RM

## Syntax

```csharp
using System;

namespace HelloWorld // namespace:  used to organize your code, and it is a container for classes and other namespaces.
{
    class Program 
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello World!");
        }
    }
}
```

## Variables

### Declaring Variables

```csharp
type variableName = value;
```

### Identifiers

* Must start with a letter or an underscore.
* Can contain letters, underscores, and digits.
* Cannot contain spaces.
* Cannot be a C# keyword.

## Data Types

### Predifined Data Types

* bool
* int
* float
* double
* char
* decimal
* string

* Long - 64-bit integer, Note: must end with an "L" or "l".
* Float - 32-bit floating point number, Note: must end with an "F" or "f".
* double - 64-bit floating point number, Note: must end with an "D" or "d".

## Type Conversion

### Implicit Conversion

```csharp
int num = 123456789;
long bigNum = num;
```

### Explicit Conversion

```csharp
double x = 1234.7;
int a;
a = (int)x;
```

### Type Casting

```csharp
double x = 1234.7;
int a;
a = Convert.ToInt32(x);
b = Convert.ToString(x);
c = Convert.ToDouble(x);
d = Convert.ToChar(x);
e = Convert.ToBoolean(x);
```

## Strings

### String Concatenation

```csharp
string firstName = "John ";
string lastName = "Doe";
string name = firstName + lastName;
```

### String Interpolation

```csharp
string firstName = "John";
string lastName = "Doe";
string name = $"My full name is: {firstName} {lastName}";
```

### String Length

```csharp
string txt = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
Console.WriteLine("The length of the txt string is: " + txt.Length);
```

### Access Strings

```csharp
string myString = "Hello";
Console.WriteLine(myString[0]); // Outputs "H"
```

### String Methods

```csharp
string myString = "Hello";
Console.WriteLine(myString.ToUpper()); // Outputs "HELLO"
Console.WriteLine(myString.ToLower()); // Outputs "hello"
Console.WriteLine(myString.IndexOf("e")); // Outputs "1"
Console.WriteLine(myString.Substring(0, 2)); // Outputs "He"
```

### Special Characters

```csharp
string txt = "We are the so-called \"Vikings\" from the north.";
```

## Conditionals

### If Statement

```csharp
if (condition) 
{
    // block of code to be executed if the condition is true
}
```

### If Else Statement

```csharp
if (condition) 
{
    // block of code to be executed if the condition is true
} 
else 
{
    // block of code to be executed if the condition is false
}
```

### If Else If Statement

```csharp
if (condition1) 
{
    // block of code to be executed if condition1 is true
} 
else if (condition2) 
{
    // block of code to be executed if the condition1 is false and condition2 is true
} 
else 
{
    // block of code to be executed if the condition1 is false and condition2 is false
}
```

### Switch Statement

```csharp
switch(expression) 
{
    case x:
        // code block
        break;
    case y:
        // code block
        break;
    default:
        // code block
        break;
}
```

## Loops

### While Loop

```csharp
while (condition) 
{
    // code block to be executed
}
```

### Do While Loop

```csharp
do 
{
    // code block to be executed
}

while (condition);
```

### For Loop

```csharp
for (statement 1; statement 2; statement 3) 
{
    // code block to be executed
}

for (int i = 0; i < 5; i++) 
{
    Console.WriteLine(i);
}
```

### Foreach Loop

```csharp
foreach (type variableName in arrayName) 
{
    // code block to be executed
}

string[] cars = {"Volvo", "BMW", "Ford", "Mazda"};
foreach (string i in cars) 
{
    Console.WriteLine(i);
}
```

## Arrays

### Declaring Arrays

```csharp
type[] arrayName;
```

### Initializing Arrays

```csharp
type[] arrayName = new type[length];
```

### Accessing Arrays

```csharp
type[] arrayName = new type[length];
arrayName[index] = value;
```

### Array Methods

```csharp
Array.Sort(arrayName);
Array.Reverse(arrayName);
```

## Methods

### Declaring Methods

```csharp
static void MethodName() 
{
    // code to be executed
}

static void MethodName(parameter1, parameter2, ...) 
{
    // code to be executed
}
```

### Calling Methods

```csharp
MethodName();
```

### Method Overloading

```csharp
static int MethodName(int x) 
{
    return 5 + x;
}

## Constructors

* A constructor in C# is a special method that is used to initialize objects. The advantage of a constructor, is that it is called when an object of a class is created. It can be used to set initial values for fields.

### Declaring Constructors

```csharp
class ClassName 
{
    public ClassName() 
    {
        // code to be executed
    }
}
```

* i.e - The constructor name must match the class name, and it cannot have a return type (like void or int).