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

> [!TIP] Why do we need data types?
> In programming, data types is an important concept. To be able to operate on variables, it is important to know something about the type. Without data types, a computer cannot safely solve this:
>
> > let x = 123 + "chicken";

> [!WARNING] Mismatched Quotes
> You cannot mismatch quotes in strings. For example, the strings 'hello" and "world' are enclosed inside one single quote and one double quote, which results in an error.
