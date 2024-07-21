# Characters

???+ info "Overview"
    
    ![Easy Badge](../../assets/images/badges/Easy.svg)
    ![CS Basics Badge](../../assets/images/badges/CS-Basics.svg)

    Characters in C# are used to represent single 16-bit Unicode characters. This includes letters, digits, punctuation, symbols, and control characters.
<br>

??? info "Useful Links"

    char:

    [https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/char](https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/char)

<br>

<br>

---

<br>

### Declaring and Initializing Characters

To declare a character variable, use the `char` keyword.

<br>

```csharp
char letter = 'A';
char symbol = '%';
```

??? info

    Characters must be enclosed in single quotes (`'`).

<br>

<br>

---

<br>

### Default Value

If a character variable is declared without an initial value, it defaults to the null character (`\0`).

<br>

```csharp
char defaultValue;
Console.WriteLine(defaultValue == '\0'); // True
```

<br>

<br>

---

<br>

### Character Methods and Properties

The `char` structure provides several methods and properties to work with characters.

<br>

#### Checking Character Types

C# provides methods to check if a character is a digit, letter, whitespace, etc.

```csharp
char ch = 'A';

bool isDigit = char.IsDigit(ch);           // False
bool isLetter = char.IsLetter(ch);         // True
bool isWhiteSpace = char.IsWhiteSpace(ch); // False
bool isUpper = char.IsUpper(ch);           // True
bool isLower = char.IsLower(ch);           // False
```

<br>

#### Character Conversion

You can convert characters to upper or lower case using `char` methods.

```csharp
char lower = 'a';
char upper = char.ToUpper(lower);  // 'A'

char upperCase = 'Z';
char lowerCase = char.ToLower(upperCase);  // 'z'
```

<br>

<br>

---

<br>

### Escaping Special Characters

Certain characters in C# have special meanings (e.g., newline, tab). These characters are represented using escape sequences.

<br>

#### Common Escape Sequences

- `\'` : Single quote
- `\"` : Double quote
- `\\` : Backslash
- `\n` : Newline
- `\r` : Carriage return
- `\t` : Tab
- `\b` : Backspace
- `\f` : Form feed

<br>

<br>