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
```

You can call it multiple times with different input to reuse the same logic.

> [!QUESTION] Question
>What does the return keyword do inside a function?
>Can you explain the difference between calling a function and defining it?

> [!SUCCESS] Tasks

>1. Create a function called greet that takes one parameter (name) and returns "Hello, [name]!"
>2. Call your greet function with different names and print the result
>3. Create a function called multiply that takes two numbers and returns their product
>4. Print out the result of calling multiply(3, 4) and multiply(7, 2)
>Bonus: Try writing a function that takes a number and returns whether it's even or odd