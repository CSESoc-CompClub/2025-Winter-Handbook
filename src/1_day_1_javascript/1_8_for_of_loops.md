## Loops – for of

The `for…of` loop iterates over the **values** of an **iterable** object (arrays, strings, Maps, Sets, etc.).

```js
let nums = [45, 52, 3, 5, 10, 11];

for (number of nums) {
  console.log(number);  // Prints the value
}
// Output:
// 45
// 52
// 3
// 5
// 10
// 11
```
> [!NOTE] Use case
> Use for…of when you need direct access to the elements of an iterable.
> If you need the indexes of an array, a traditional for loop or array.entries() is a better choice.
> To iterate over object properties, use for…in or Object.keys() / Object.entries().