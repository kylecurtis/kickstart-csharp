# Booleans

???+ info "Overview"

    ![Easy Badge](../../assets/images/badges/Easy.svg)
    ![CS Basics Badge](../../assets/images/badges/CS-Basics.svg)

    A boolean is a data type that can hold one of two values: `true` or `false`. It is used in decision-making statements and to control the flow of the program based on logical conditions.

<br>

??? info "Useful Links"

    bool:

    - [https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/bool](https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/bool)


<br>

<br>

---

<br>


### Declaring and Initializing Booleans

To declare a boolean variable, use the `bool` keyword. You can also initialize it at the time of declaration.

<br>

#### Boolean True

```csharp
bool isSunny = true;
```

<br>

#### Boolean False

```csharp
bool isRaining = false;
```

<br>

#### Boolean Struct

```csharp
System.Boolean isOffline = false;
```

??? info

    `System.Boolean` is the struct which the `bool` keyword references. This is not the recommended way to declare a boolean.

    [https://learn.microsoft.com/en-us/dotnet/api/system.boolean](https://learn.microsoft.com/en-us/dotnet/api/system.boolean)

<br>

<br>

---

<br>

### Default Value

If a boolean variable is declared without an initial value, it defaults to `false`.

<br>

```csharp
bool defaultValue;
Console.WriteLine(defaultValue); // False
```

<br>

<br>