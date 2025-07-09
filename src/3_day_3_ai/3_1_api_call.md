# Part 1: Make A Direct API Call
> [!IMPORTANT] Revision
> In this section, we will revise how to make an API call
> [Link to APIs](https://github.com/public-apis/public-apis?tab=readme-ov-file#programming)

> [!SUCCESS] Tasks
> 1. Click on `api-call.js` in visual studio code
> 2. Follow the instruction below to make an API Call

### Define An `async` Function
> [!INFO] Info
> `async` means this function can use `await` inside it.

> [!TIP]  Tip
> ``` Javascript
>   async function nameOfFunction()
> ```

### `try` and `catch` block
> [!INFO] Info
> - This is where you put code that **might fail**, in this case your API Call.
> - If something goes wrong, your program will jump to the `catch` block.

> [!TIP]  Tip 
> ```javascript
>    try {
>        ...
>    } catch (error) {
>        ...
>    }
> ```

### Send A Request to the API
> [!INFO] Info 
> - `fetch(...)` sends a GET request to the URL.
> - `await` means "wait for the response before continuing."
>    

> [!TIP]  Tips
> ```javascript
>        const response = await fetch('<url of your API>');
>    ```

### Parse the JSON Response
> [!INFO] Info
> The API returns something like:
> ```JSON
>    {
>    "data": ["Response from AI"]
>    }
> ```
> - `await response.json()` reads the body of the response and turns it into a JavaScript object.
> - The result is stored in the `data` variable.

> [!TIP] Tip
> ```Javascript
>   const data = await response.json();
> ```

### Print the Response to the Console
> [!INFO] Info
> - `data.data` is an array of facts.
> - `data.data[0]` gives you the first fact.

> [!TIP]  Tip
> ```javascript
>   console.log(...);
> ```

### Throw An Error
> [!INFO] Info
> - If `fetch` fails (e.g. no internet, server down), the code will jump to `catch` and print the error message.
> - You'll want see a helpful message like:
```
    Something went wrong: TypeError: Failed to fetch
```
> [!TIP]  Tip
> ```javascript
>    console.error('Something went wrong:', error);
> ```

### Call the function
> [!INFO] Info
> - This runs everything we just wrote.
> - It will print a random cat fact or an error in the console.

> [!TIP]  Tip
> ```javascript
> nameOfFunction();
> ```
