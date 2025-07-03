# Operators

There are different types of JavaScript operators. The primary types of operators you'll encounter are:

- Arithmetic Operators
- Assignment Operators
- Comparison Operators
- Logical Operators

## Arithmetic Operators

| **Operator** | **Meaning**                                                     | **Example**                   |
| ------------ | --------------------------------------------------------------- | ----------------------------- |
| +            | Addition: Adds two values                                       | let add = 250 + 170;          |
| -            | Subtraction: Minuses one value from another                     | let sub = 500 - 80;           |
| \*           | Multiplication: Multiplies two numbers                          | let mul = 5 \* 8;             |
| /            | Division: Divides one number by another                         | let splitCandy = 100 / 12;    |
| %            | Modulo: Returns the remainder of dividing one number by another | let leftOverCandy = 100 % 12; |

## Assignment Operators

| **Operator** | **Meaning**                                                        | **Example**         |
| ------------ | ------------------------------------------------------------------ | ------------------- |
| =            | Equals: Assigns a value                                            | x = y               |
| +=           | Plus Equals: Assigns the original value plus the new value         | x += y // x = x + y |
| -=           | Minus Equals: Assigns the original value minus the new value       | x -= y // x = x - y |
| \*=          | Multiply Equals: Assigns the original value times the new value    | x _= y // x = x _ y |
| /=           | Divide Equals: Assigns the original value divided by the new value | x /= y // x = x / y |
| %=           | Modulo Equals: Assigns the original value modulo the new value     | x %= y // x = x % y |

## Comparison Operators

Comparison operators are used in logical statements to determine equality or difference between variables or values.
Given that x = 5, the table below explains the comparison operators:

| **Operator** | **Description**          | **Comparison** |
| ------------ | ------------------------ | -------------- |
| ===          | equal to                 | x === 5 (true) |
| !==          | not equal                | x !== 8 (true) |
| >            | greater than             | x > 8 (false)  |
| <            | less than                | x < 8 (true)   |
| >=           | greater than or equal to | x >= 8 (false) |
| <=           | less than or equal to    | x <= 8 (true)  |

> [!IMPORTANT]
> Notice that we are using triple equals sign (===) instead of double equals sign (==). This is called strict equality and is used for checking that both sides have the same type.

## Logical Operators

Logical operators are used to determine the logic between variables or values.
Given that x = 6 and y = 3, the table below explains the logical operators:

| **Operator** | **Description** | **Example**                   |
| ------------ | --------------- | ----------------------------- |
| &&           | and             | (x < 10 && y > 1) is true     |
| \|\|         | or              | (x == 5 \|\| y == 5) is false |
| !            | not             | !(x == y) is true             |
