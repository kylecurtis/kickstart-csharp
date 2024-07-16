# Variables & Constants

???+ info "Overview"

    ![Easy Badge](../../assets/images/badges/Easy.svg)
    ![CS Basics Badge](../../assets/images/badges/CS-Basics.svg)

    In C#, variables and constants are fundamental elements used to store and manage data. Understanding how to declare, initialize, and use them is crucial for writing effective and efficient code.

<br>

<br>

---

<br>

### Variable Declaration and Initialization

<br>

???+ info "What is a Variable?"

    A **variable** is a named storage location in memory that holds a value which can be changed during the execution of a program. Variables are used to store data that your program can manipulate.

<br>

#### Declaring Variables

To declare a variable in C#, you need to specify the data type and the variable name. Here is the syntax for declaring a variable:

```csharp
dataType variableName;
```

<br>

#### Initializing Variables

Initialization is the process of assigning a value to a variable at the time of declaration. Here is the syntax for declaring and initializing a variable:

```csharp
dataType variableName = value;
```

<br>

#### Variable Example

```csharp
int numOfGuests = 12;
```

??? info

    This example declares an [integer](./integers.md) (whole number) variable named `num_of_guests` and initializes it with the value 12.

    [Naming Conventions](https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/coding-style/identifier-names#naming-conventions) recommend **camelCase** for local variables (i.e. every word is capitalized except for the first).

<br>

#### Variable Scope

The scope of a variable is the region of the program where the variable is accessible. Variables can be declared inside methods, classes, or blocks of code. The scope determines the lifetime and visibility of the variable.

<br>

<br>

---

<br>

### Constants And Read-Only Fields

<br>

???+ info "What is a Constant?"

    A **constant** is a variable whose value cannot be changed once it has been assigned. Constants are used to store values that remain constant throughout the execution of the program.

<br>

#### Declaring Constants

To declare a constant, use the `const` keyword:

```csharp
const dataType ConstantName = value;
```

<br>

#### Example

```csharp
const int DaysInWeek = 7;
```

??? info

    This example declares an [integer](./integers.md) constant named `DaysInWeek` and initializes it with the value 7.

    [Naming Conventions](https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/coding-style/identifier-names#naming-conventions) recommend **PascalCase** for constants (i.e. every word is capitalized).

<br>

<br>

---

<br>

### Read-Only Fields

<br>

???+ info "What is a Read-Only Field?"

    Read-only fields are similar to constants, but their values can be assigned at runtime, typically in the constructor of a class. Once assigned, their values cannot be changed.

<br>

#### Declaring Read-Only Fields

To declare a read-only field, use the `readonly` keyword:

```csharp
readonly dataType fieldName;
```

<br>

#### Example

```csharp
class Circle
{
    public readonly float Radius;
    
    public Circle(float radius)
    {
        Radius = radius;
    }
}
```

??? info

    This example declares a read-only field named `Radius`.

    The constructor `public Circle(float radius)` initializes the `Radius` field. After this initialization, the value of `Radius` cannot be changed.

    [Naming Conventions](https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/coding-style/identifier-names#naming-conventions) recommend **PascalCase** for constant (read-only) fields (i.e. every word is capitalized).

<br>

<br>