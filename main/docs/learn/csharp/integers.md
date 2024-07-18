# Integers

???+ info "Overview"

    ![Easy Badge](../../assets/images/badges/Easy.svg)
    ![CS Basics Badge](../../assets/images/badges/CS-Basics.svg)

    Integers are whole numbers which can be negative, and are one of the most commonly used data types in programming. 

    In C#, there are several types of integer data types, each suited for different purposes depending on the range and size of the values you need to store.

    - **Signed:** Negative sign allowed (-10, -5, 0, etc).

    - **Unsigned:** Negative sign *not* allowed (0, 5, 10, etc).

<br>

??? info "Useful Links"

    Integral Numeric Types:

    - [https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/integral-numeric-types](https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/integral-numeric-types)

<br>

<br>

---

<br>

### sbyte

Represents an 8-bit signed integer.

<br>

???+ info "Quick Info"

    - **Type:** Signed
    - **Size:** 8 bits (1 byte)
    - **Range:** -128 to 127
    - **Default Value:** 0

<br>

#### SByte Example

```csharp
sbyte sbyteMin = -128;
```

??? info

    Use the `sbyte` keyword to declare a signed byte (recommended).


<br>

#### SByte Struct

```csharp
System.SByte sbyteMax = 127;
```

??? info

    `System.SByte` is the struct which the `sbyte` keyword references. This is not the recommended way to declare a signed byte.

    [https://learn.microsoft.com/en-us/dotnet/api/system.sbyte](https://learn.microsoft.com/en-us/dotnet/api/system.sbyte)


<br>

<br>

---

<br>

### byte

Represents an 8-bit unsigned integer.

<br>

???+ info "Quick Info"

    - **Type:** Unsigned
    - **Size:** 8 bits (1 byte)
    - **Range:** 0 to 255
    - **Default Value:** 0

<br>

#### Byte Example

```csharp
byte byteMin = 0;
```

??? info

    Use the `byte` keyword to declare an unsigned byte (recommended).

<br>

#### Byte Struct 

```csharp
System.Byte byteMax = 255;
```
??? info

    `System.Byte` is the struct which the `byte` keyword references. This is not the recommended way to declare an unsigned byte. 

    [https://learn.microsoft.com/en-us/dotnet/api/system.byte](https://learn.microsoft.com/en-us/dotnet/api/system.byte)
  
<br>

<br>

---

<br>

### short

Represents a 16-bit signed integer.

<br>

???+ info

    - **Type:** Signed
    - **Size:** 16 bits (2 bytes)
    - **Range:** -32,768 to 32,767
    - **Default Value:** 0

<br>

#### Short Example

```csharp
short shortMin = -32_768;
```

??? info

    Use the `short` keyword to declare a signed short (recommended).

<br>

#### Int16 Struct

```csharp
System.Int16 shortMax = 32_767;
```

??? info

    `System.Int16` is the struct which the `short` keyword references. This is not the recommended way to declare a signed short.

    [https://learn.microsoft.com/en-us/dotnet/api/system.int16](https://learn.microsoft.com/en-us/dotnet/api/system.int16)


<br>

<br>

---

<br>

### ushort 

Represents a 16-bit unsigned integer.

<br>

???+ info

    - **Type:** Unsigned
    - **Size:** 16 bits (2 bytes)
    - **Range:** 0 to 65,535
    - **Default Value:** 0

<br>

#### Ushort Example

```csharp
ushort ushortMin = 0;
```

??? info

    Use the `ushort` keyword to declare an unsigned short (recommended).

<br>

#### UInt16 Struct

```csharp
System.UInt16 ushortMax = 65_535;
```

??? info

    `System.UInt16` is the struct which the `ushort` keyword references. This is not the recommended way to declare an unsigned short.

    [https://learn.microsoft.com/en-us/dotnet/api/system.uint16](https://learn.microsoft.com/en-us/dotnet/api/system.uint16)

<br>

<br>

---

<br>

### int

Represents a 32-bit signed integer.

<br>

???+ info

    - **Type:** Signed
    - **Size:** 32 bits (4 bytes).
    - **Range:** -2,147,483,648 to 2,147,483,647.
    - **Default Value:** 0.

<br>

#### Int Example

```csharp
int minInt = -2_147_483_648;
```

??? info

    Use the `int` keyword to declare a signed int (recommended).

<br>

#### Int32 Struct

```csharp
System.Int32 maxInt = 2_147_483_647;
```

??? info

    `System.Int32` is the struct which the `int` keyword references. This is not the recommended way to declare a signed int.

    [https://learn.microsoft.com/en-us/dotnet/api/system.int32](https://learn.microsoft.com/en-us/dotnet/api/system.int32)

<br>

<br>

---

<br>

### uint

Represents a 32-bit unsigned integer.

<br>

???+ info "Quick Info"

    - **Type:** Unsigned
    - **Size:** 32 bits (4 bytes)
    - **Range:** 0 to 4,294,967,295
    - **Default Value:** 0

<br>

#### UInt Example

```csharp
uint uintMin = 0;
```

??? info

    Use the `uint` keyword to declare an unsigned int (recommended).

<br>

#### UInt32 Struct

```csharp
System.UInt32 uintMax = 4_294_967_295;
```

??? info

    `System.UInt32` is the struct which the `uint` keyword references. This is not the recommended way to declare an unsigned int.

    [https://learn.microsoft.com/en-us/dotnet/api/system.uint32](https://learn.microsoft.com/en-us/dotnet/api/system.uint32)

<br>

<br>

---

<br>


### long

Represents a 64-bit signed integer.

<br>

???+ info "Quick Info"

    - **Type:** Signed
    - **Size:** 64 bits (8 bytes)
    - **Range:** -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807
    - **Default Value:** 0L

<br>

#### Long Example

```csharp
long longMin = -9_223_372_036_854_775_808L;
```

??? info

    Use the `long` keyword to declare a signed long (recommended).

    Use the `L` or `l` suffix at the end of the initialized value (required).

<br>

#### Int64 Struct

```csharp
System.Int64 longMax = 9_223_372_036_854_775_807L;
```

??? info

    `System.Int64` is the struct which the `long` keyword references. This is not the recommended way to declare a signed long.

    [https://learn.microsoft.com/en-us/dotnet/api/system.int64](https://learn.microsoft.com/en-us/dotnet/api/system.int64)

<br>

<br>

---

<br>

### ulong

Represents a 64-bit unsigned integer.

<br>

???+ info "Quick Info"

    - **Type:** Unsigned
    - **Size:** 64 bits (8 bytes)
    - **Range:** 0 to 18,446,744,073,709,551,615
    - **Default Value:** 0UL

<br>

#### Ulong Example

```csharp
ulong ulongMin = 0UL;
```

??? info

    Use the `ulong` keyword to declare an unsigned long (recommended).

    Use the `UL` or `ul` suffix at the end of the initialized value (required).

<br>

#### UInt64 Struct

```csharp
System.UInt64 ulongMax = 18_446_744_073_709_551_615UL;
```

??? info

    `System.UInt64` is the struct which the `ulong` keyword references. This is not the recommended way to declare an unsigned long.

    [https://learn.microsoft.com/en-us/dotnet/api/system.uint64](https://learn.microsoft.com/en-us/dotnet/api/system.uint64)

<br>

<br>

---

<br>

### BigInteger

<br>

???+ info

    For situations requiring integer values larger than what `long` or `ulong` can store, C# provides the `BigInteger` type in the `System.Numerics` namespace. 

    `BigInteger` can represent arbitrarily large integers.

<br>

#### BigInteger Example

```csharp title="~/Integers/Program.cs"
using System.Numerics;

namespace Integers;

class Program
{
    static void Main(string[] args)
    {
        BigInteger bigValue = BigInteger.Parse("123456789012345678901234567890");
        Console.WriteLine(bigValue);
    }
}
```

??? success "Run"

    123456789012345678901234567890

    Process finished with exit code 0.

<br>

<br>