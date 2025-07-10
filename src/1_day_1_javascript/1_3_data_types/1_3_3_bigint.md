## JavaScript BigInt

**BigInt** is a type of number that can represent very large or very small integers beyond the range of the regular number data type. A BigInt number is created by appending n to the end of an integer.

> [!INFO] Number Range
> The regular number data type can handle values less than (2^53 - 1) and greater than -(2^53 - 1).

> [!WARNING] Mixing Datatypes
> You can't mix BigInt and number values (for instance, by performing arithmetic operations between them).

```js
// BigInt value
let value = 900719925124740998n;

// BitInt and number cannot be added
let sum = value + 123;
console.log(sum); // TypeError: Cannot mix BigInt and other types, use explicit conversions

// add two big integers
let sum2 = value + 123n;
console.log(sum2); // success
```
