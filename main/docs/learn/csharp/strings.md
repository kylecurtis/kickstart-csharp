# Strings 

???+ info "Overview"
    
    ![Easy Badge](../../assets/images/badges/Easy.svg)
    ![CS Basics Badge](../../assets/images/badges/CS-Basics.svg)

    In C#, a string is an object of the `String` class, which represents a sequence of characters and is stored as a contiguous block of memory. Strings in C# are immutable, meaning once a string is created, it cannot be modified. Any operations that appear to modify a string actually result in the creation of a new string.

<br>

??? info "Useful Links"

    strings:

    - [https://learn.microsoft.com/en-us/dotnet/csharp/programming-guide/strings/](https://learn.microsoft.com/en-us/dotnet/csharp/programming-guide/strings/)


<br>

<br>

---

<br>

### Empty String

A predefined constant representing an empty (i.e. zero-length) string.

<br>

#### Correct Way

```csharp
string emptyString = String.Empty;
```

??? info

    This method is the preferred way to initialize an empty string.

<br>

#### Incorrect Way

```csharp
string emptyString = "";
```

??? info

    This method is essentially what `String.Empty` does, but it can cause a NullReferenceException, whereas `String.Empty` does not.

    Do not use this method whenever an empty string is needed.


<br>

<br>

---

<br>

### String Literal

The most common and direct way to create a string is with a literal.

<br>

```csharp
string planet = "Earth";
```

??? info

    Strings must be enclosed in double quotes (`""`).

<br>

<br>

---

<br>

### String Interpolation

Prefixed with `$`, string interpolation is a concise way to embed variables and expressions directly within strings using curly brackets (`{}`).

<br>

#### Variable Interpolation

```csharp

// Variable
string greeting = "Hello";

// Variable Interpolation
string result = $"{greeting}!"; // Hello!
```

<br>

#### Expression Interpolation

```csharp
string total = $"{1 + 1}"; // 2
```

??? info

    Although anything that is enclosed between curly brackets are technically called "expressions", interpolation can also allow for calculations with operators (such as mathematical expressions).

<br>

<br>

---

<br>

### Verbatim String Literals

Prefixed with `@`, verbatim strings interpret backslashes literally (ideal for paths, regular expressions, and multi-line strings).

<br>

```csharp
string path = @"C:\Windows\Fonts";
```

<br>

<br>

---

<br>

### Verbatim string interpolation

You can also mix interpolation with verbatim string literals by using the prefix `$@` or `@$`.

```csharp
// Variable
string username = "Adam";

// Verbatim String Interpolation
string directory = $@"C:\Users\{username}\Desktop";
```


<br>

<br>

---

<br>
