## Loops – for in

The `for…in` loop iterates over the **properties (keys/indexes)** of an object.  
When used on arrays, it returns the **indexes** (not the values directly).

```js
let nums = [45, 52, 3, 5, 10, 11];

for (index in nums) {
  console.log(index);        // Prints the index
  console.log(nums[index]);  // Prints the value
}
// Output:
// 0
// 45
// 1
// 52
// 2
// 3
// 3
// 5
// 4
// 10
// 5
// 11
```

> [!NOTE] Use case
> for…in is typically used for objects. When looping through arrays, prefer for…of or a traditional for loop to avoid unexpected behavior with inherited properties.
> let person = { name: "Jamie", age: 22, student: true };

```
for (key in person) {
  console.log(key);          // Prints the property name
  console.log(person[key]);  // Prints the value of that property
}
// Output:
// name
// Jamie
// age
// 22
// student
// true
```