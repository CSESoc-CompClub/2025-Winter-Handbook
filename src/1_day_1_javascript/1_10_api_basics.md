# Basics of APIs

- Stands for "Application Programming Interface".
- Allows us to communicate with websites & programs we don't control.


> [!TIP]
> There are lots of free APIs out there! Try the following page for some.
>
> [https://github.com/public-apis/public-apis](https://github.com/public-apis/public-apis)

# Query parameters

Query parameters come in parameter/value pairs -- We pass these to the API in order to control what it will return to us. Parameters are always strings, but values can be anything.

## Query parameter syntax

When writing a query parameter directly in a URL, we indicate individual parameter/value pairs with "?parameter=value", and put multiple together with "&". Some examples, with a base URL of <https://meowfacts.herokuapp.com/>:

- <https://meowfacts.herokuapp.com/?count=3>
- <https://meowfacts.herokuapp.com/?lang=ukr>
- <https://meowfacts.herokuapp.com/?lang=ukr&count=3>

Order does not matter. The following is the same as the last example.

- <https://meowfacts.herokuapp.com/?count=3&?lang=ukr>
