# Data Types

JavaScript has 8 datatypes:

- **String**
- **Number**
- **Bigint**
- **Boolean**
- Undefined
- Null
- Symbol
- Object

In this workshop, we are only focusing on the ones in bold.

| **Data Type** | **Description**                       | **Examples**            |
| ------------- | ------------------------------------- | ----------------------- |
| String        | Textual data                          | "hello", "hello world!" |
| Number        | An integer or a floating-point number | 3, 3.234, 3e-2          |
| BigInt        | An integer with arbitrary precision   | 900719925124740999n, 1n |
| Boolean       | Any of two values: true or false      | true and false          |

> [!TIP]
> In programming, data types is an important concept. To be able to operate on variables, it is important to know something about the type. Without data types, a computer cannot safely solve this:
>
> > let x = 123 + "chicken";

## JavaScript String

A string represents textual data. It contains a sequence of characters. For example, "hello", "JavaScript", etc. In JavaScript, strings are surrounded by quotes:

```js
// string enclosed within single quotes
let fruit = "apple";
console.log(fruit);

// string enclosed within double quotes
let country = "banana";
console.log(country);

// string enclosed within backticks
let result = `cherry`;
console.log(result);
```

> [!WARNING]
> You cannot mismatch quotes in strings. For example, the strings 'hello" and "world' are enclosed inside one single quote and one double quote, which results in an error.

## JavaScript Number

In JavaScript, the **number** type represents numeric values (both integers and floating-point numbers).

1. Integers - Numeric values without any decimal parts. Example: 3, -74, etc.
2. Floating-Point - Numeric values with decimal parts. Example: 3.15, -1.3, etc.

```js
// integer value
let integer_number = -3;
console.log(integer_number);

// floating-point value
let float_number = 3.15;
console.log(float_number);
```

## JavaScript BigInt

**BigInt** is a type of number that can represent very large or very small integers beyond the range of the regular number data type. A BigInt number is created by appending n to the end of an integer.

> [!INFO]
> The regular number data type can handle values less than (2^53 - 1) and greater than -(2^53 - 1).

> [!WARNING]
> You can't mix BigInt and number values (for instance, by performing arithmetic operations between them).

```js
// BigInt value
let value = 900719925124740998n;

// BitInt and number cannot be added
let sum = value + 123; 
console.log(sum); // TypeError: Cannot mix BigInt and other types, use explicit conversions

// add two big integers
let sum2 = value + 123n;
console.log(result1);  // success
```

## JavaScript Boolean

A **Boolean** data can only have one of two values: true or false.

```js
let isRaining = true;
console.log(dataChecked);  // true

let isWeekend = false;
console.log(valueCounted);  // false
```
