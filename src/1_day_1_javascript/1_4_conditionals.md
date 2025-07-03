# Conditionals

Conditional statements are used to perform different actions based on different conditions.

- Use `if` to specify a block of code to be executed, if a specified condition is true
- Use `else` to specify a block of code to be executed, if the same condition is false
- Use `else if` if to specify a new condition to test, if the first condition is false
- Use `switch` to specify many alternative blocks of code to be executed

## if statement

Use the `if` statement to specify a block of JavaScript code to be executed if a condition is true.

```js
if (condition) {
  //  block of code to be executed if the condition is true
}

// make a "Good day" greeting if the hour is less than 18:00:
if (hour < 18) {
  greeting = "Good day";
  console.log(greeting);
}
```

> [!IMPORTANT]
> Note that if is in lowercase letters. Uppercase letters (If or IF) will generate a JavaScript error.

## else statement

Use the `else` statement to specify a block of code to be executed if the condition is false.

```js
if (condition) {
  //  block of code to be executed if the condition is true
} else {
  //  block of code to be executed if the condition is false
}

// if the hour is less than 18, create a "Good day" greeting, otherwise "Good evening":
if (hour < 18) {
  greeting = "Good day";
} else {
  greeting = "Good evening";
}
```

## else if statement

Use the `else` if statement to specify a new condition if the first condition is false.

```js
if (condition1) {
  //  block of code to be executed if condition1 is true
} else if (condition2) {
  //  block of code to be executed if the condition1 is false and condition2 is true
} else {
  //  block of code to be executed if the condition1 is false and condition2 is false
}

// If time is less than 10:00, create a "Good morning" greeting, if not, but time is less than 20:00, create a "Good day" greeting, otherwise a "Good evening":
if (time < 10) {
  greeting = "Good morning";
} else if (time < 20) {
  greeting = "Good day";
} else {
  greeting = "Good evening";
}
```

## switch statement

A `switch` statement allows you to execute different blocks of code based on the value of a variable. It’s an alternative to using multiple if else statements when you’re checking one variable against several possible values.

How it works:

1. The switch expression is evaluated once
2. The value of the expression of compared with the values of each case
3. If there is a match, the associated code black is executed
4. If there is no match, the default code block is executed

```js
switch (expression) {
  case x:
    // code block
    break;
  case y:
    // code block
    break;
  default:
  // code block
}

// check the value of the monster variable and execute different code based on which monster it is
let monster = "Werewolf";

switch (monster) {
  case "Ghost":
    console.log("A ghost appears, floating silently through the trees!");
    break;
  case "Vampire":
    console.log("A vampire emerges from the shadows, thirsty for blood!");
    break;
  case "Werewolf":
    console.log("A werewolf howls at the full moon and charges toward you!");
    break;
  case "Zombie":
    console.log("A zombie shuffles toward you, groaning for brains!");
    break;
  default:
    console.log("Unknown monster");
}
```

> [!INFO]
> The default keyword specifies the code to run if there is no case match. It is not necessary to break the last case in a switch block. The block breaks ends there anyway.

> [!NOTE]
> When JavaScript reaches a break keyword, it breaks out of the switch block.
> If you omit the break statement, execution will continue to the next case regardless of whether its condition matches.
