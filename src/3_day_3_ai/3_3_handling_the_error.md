# Handling the Error

> [!INFO] Info
> - If `fetch` fails (e.g. no internet, server down), the code will jump to `catch` and print the error message.
> - You'll want see a helpful message like:
> ```
>   Something went wrong: TypeError: Failed to fetch
> ```

~~~admonish tip collapsible=true, title='<span style="color:#00e7c1">Tip</span>'
<b><span style="color: #00e7c1"></span></b>
```javascript
console.error('Something went wrong:', error);
```
~~~
