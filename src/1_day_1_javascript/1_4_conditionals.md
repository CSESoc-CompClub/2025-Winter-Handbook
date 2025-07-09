# Conditionals

Conditional statements are used to perform different actions based on different conditions.

- Use `if` to specify a block of code to be executed, if a specified condition is true
- Use `else` to specify a block of code to be executed, if the same condition is false
- Use `else if` if to specify a new condition to test, if the first condition is false
- Use `switch` to specify many alternative blocks of code to be executed

---

> [!SUCCESS] Your Turn: Conditionals Task
> Set your favorite color in the variable below then use conditionals to print a message:
>
> ```js
> let favoriteColor = "red"; // try changing this to blue, green, etc
> ```
>
> - If the color is **Red** -> print `Roses are red :)`
> - If the color is **Blue** -> print `The sky is blue`
> - For any other color -> print `That's a cool color!`

> [!SUCCESS] Your Turn: Switch Task
> Rewrite this if...else if chain using a switch statement
>
> ```js
> potion = "healing"; // try changing this to other values
> if (potion === "healing") {
>   console.log("Restores health!");
> } else if (potion === "invisibility") {
>   console.log("You disappear!");
> } else if (potion === "strength") {
>   console.log("You feel powerful!");
> } else if (potion === "poison") {
>   console.log("Ouch! Toxic!");
> } else {
>   console.log("Unknown potion!");
> }
> ```
