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

> [!INFO] Default Case
> The default keyword specifies the code to run if there is no case match. It is not necessary to break the last case in a switch block. The block breaks ends there anyway.

> [!NOTE] Break Statement
> When JavaScript reaches a break keyword, it breaks out of the switch block.
> If you omit the break statement, execution will continue to the next case regardless of whether its condition matches.
