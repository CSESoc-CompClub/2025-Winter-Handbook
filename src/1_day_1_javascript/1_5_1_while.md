# While Loops

The while loop loops through a block of code as long as a specified condition is true.

```js
while (condition) {
  // code block to be executed
}

// This loop will run, over and over again, as long as the variable i is less than 10:
while (i < 10) {
  text += "The number is " + i;
  i++;
}
// Output:
// The number is 0
// The number is 1
// The number is 2
// The number is 3
// The number is 4
// The number is 5
// The number is 6
// The number is 7
// The number is 8
// The number is 9

// This loop counts down the days until winter. It runs as long as daysUntilWinter is greater than 0:
let daysUntilWinter = 5;
while (daysUntilWinter > 0) {
  console.log("Days until Winter: " + daysUntilWinter);
  daysUntilWinter--; // Decrease the counter by 1
}
console.log("It's Winter!");
// Output:
// Days until Winter: 5
// Days until Winter: 4
// Days until Winter: 3
// Days until Winter: 2
// Days until Winter: 1
// It's Winter!
```

> [!CAUTION] Infinite Loop
> If you forget to update the variable in the loop condition, the loop might never end (infinite loop). It can make your program freeze or hang because it keeps running forever.
