# Hello, World!

The "Hello, World!" program is a classic introduction to a new programming language. It is the simplest program you can write and serves as a good starting point for understanding the basic structure and syntax of C#.

<br>

<br>

---

<br>

## Writing the Program

<br>

In C#, every application starts with a `Main` method. This method is the entry point of your program. 

Here is a basic example of a "Hello, World!" program in C#:

<br>

```csharp title="~/HelloWorld/Program.cs"
using System;

namespace HelloWorld
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello, World!");
        }
    }
}
```

??? success "Run"

    Hello, World!

    Process finished with exit code 0.


<br>

<br>

---

<br>

## Code Breakdown

<br>

```csharp 
using System;
```

??? info
    The `using` keyword is used to include the `System` namespace in your program. Namespaces in C# provide a way to organize large code projects. The `System` namespace contains fundamental classes for basic input-output operations.

<br>

```csharp
namespace HelloWorld
```

??? info
    The `namespace` keyword is used to declare a scope that contains a set of related objects. In this case, we define a namespace called `HelloWorld`. This helps to organize code and prevent naming conflicts.

<br>

```csharp
class Program
```
??? info
    The `class` keyword is used to define a class. In C#, everything is encapsulated within classes. Here, we define a class named `Program`.

<br>

```csharp
static void Main(string[] args)
```
??? info
    The `Main` method is the entry point of any C# application. The `static` keyword means that this method belongs to the class itself rather than an instance of the class. `void` means that this method does not return a value. The `string[] args` parameter is used to accept command-line arguments.

<br>

```csharp
Console.WriteLine("Hello, World!");
```

??? info
    This line outputs the string "Hello, World!" to the console. `Console` is a class in the `System` namespace that provides methods for input-output operations. `WriteLine` is a method that prints a message to the console and then moves to the next line.

<br>

<br>