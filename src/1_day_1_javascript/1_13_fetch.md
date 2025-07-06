# Fetch

`fetch` is the function we use to make an API call in Javascript.

In its most simple form, we simply call fetch using `await` (and then `await` again on some of the contents, as the thing returned by `fetch` is quite complex and we only need a little bit of it):
```js
let response = await fetch("https://meowfacts.herokuapp.com");
let data = await response.json();
console.log(data);
```
`.json()` converts the response from `fetch` into data we can use.

# Query parameters

To add query parameters, we need to manually add them to the URL. (See the Query Parameters page for how to do this!).

```js
let response = await fetch("https://meowfacts.herokuapp.com/?count=3")
let data = await response.json()
console.log(data)
```


## Automagical query parameters

There is a method of automatically adding query parameters, but it's out of scope for this course. We provide it here anyway - perhaps you could try and figure out how it works? If not, you can use it as much as you like anyway.

```js
let params = new URLSearchParams();
params.append("count", 3)

let response = await fetch(`https://meowfacts.herokuapp.com/${params}`)
let data = await response.json()
console.log(data)
```

Note the backticks \` instead of quotes "!
