# Floats

???+ info "Overview"

    ![Easy Badge](../../assets/images/badges/Easy.svg)
    ![CS Basics Badge](../../assets/images/badges/CS-Basics.svg)

    Floating-point numbers are used to represent real numbers that have fractional parts. In C#, there are three main floating-point types: `float`, `double`, and `decimal`. Each of these types has different ranges and precision, suitable for various purposes.

<br>

??? info "Useful Links"

    Floating-point numeric types:

    - [https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/floating-point-numeric-types](https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/floating-point-numeric-types)


<br>

<br>

---

<br>

### float

Represents a single-precision floating-point number.

<br>

???+ info "Quick Info"

    - **Size:** 32 bits (4 bytes)
    - **Precision:** 7 digits
    - **Range:** ±1.5 × 10^−45 to ±3.4 × 10^38
    - **Default Value:** 0.0F
    - **Suffix:** `f` or `F`

<br>

#### Float Example

```csharp
float floatNum = 32.0F;
```

<br>

<br>

---

<br>

### double

Represents a double-precision floating-point number.

<br>

???+ info "Quick Info"

    - **Size:** 64 bits (8 bytes)
    - **Precision:** 15-16 digits
    - **Range:** ±5.0 × 10^−324 to ±1.7 × 10^308
    - **Default Value:** 0.0d
    - **Suffix:** `d` or `D` (default for floating-point literals)

<br>

#### Double Example

```csharp
double doubleNum = 123.45D;
```

<br>

<br>

---

<br>

### decimal

Represents a decimal floating-point number.

<br>

???+ info "Quick Info"

    - **Size:** 128 bits (16 bytes)
    - **Precision:** 28-29 significant digits
    - **Range:** ±1.0 × 10^−28 to ±7.9 × 10^28
    - **Default Value:** 0.0m
    - **Suffix:** `m` or `M`

<br>

#### Decimal Example

```csharp
decimal price = 4.99M;
```

<br>

<br>

---

<br>

### IEEE Specifications

<br>

???+ info

    C# floating-point types are based on the IEEE 754 specification for binary floating-point arithmetic. This specification defines the format and operations for floating-point numbers to ensure consistency across different computing platforms.

    - **IEEE 754 Single Precision:** Used by `float`
    - **IEEE 754 Double Precision:** Used by `double`
    - **IEEE 754 Decimal:** Used by `decimal`

<br>

<br>

---

<br>

### Precision and Rounding Issues

Floating-point numbers have limited precision, which can lead to rounding errors in calculations. This is due to the way floating-point numbers are represented in binary format.

<br>

#### Example of Precision Issues

```csharp
double a = 0.1;
double b = 0.2;
double sum = a + b;

Console.WriteLine(sum == 0.3); // Output: False 
```

??? info

    In this example, the expected result is `True`, but due to precision limitations, the actual result is `False` (caused by the result of the calculation not adding up to exactly 0.3).

<br>

#### Using Decimal for High Precision

For applications requiring high precision, such as financial calculations, use the `decimal` type instead of `float` or `double`.

<br>

#### Example

```csharp
decimal price = 19.99m;
decimal tax = 0.08m;
decimal total = price + (price * tax);

Console.WriteLine(total); // Output: 21.5892
```

<br>

<br>