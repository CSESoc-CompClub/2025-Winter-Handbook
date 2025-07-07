# What are functions?

Functions are a useful tool where we can store code separately so we don’t have to rewrite it. This makes coding easier in the long run, whenever you need to repeat a block of code you’ve already written, just call the function instead!

---

# How to Define a Function

To define a function in JavaScript:

1. Use the `function` keyword  
2. Give it a **name**  
3. List **parameters** inside parentheses (`(…)`)  
4. Write the **body** between `{ … }`  
5. Use `return` to specify the **output**  

```js
function addNums(a, b) {
  return a + b;
}

let result1 = addNums(4, 5);
let result2 = addNums(10, 11);

console.log(result1); // 9
console.log(result2); // 21
addNums takes 2 arguments each time.

You can call it multiple times with different input to reuse the same logic.