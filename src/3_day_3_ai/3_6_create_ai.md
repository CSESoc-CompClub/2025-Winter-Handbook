# Create A New Slash Command

**Now we want to be able to call the Open Ai using our discord bot. Here we will implement a new slash command: `/ask`.**

TASK
Create a slash command for our bot.
- 

Create a new file called ai.js in the commands/utilities folder. 

```js
import { SlashCommandBuilder } from 'discord.js';

const data = new SlashCommandBuilder()
  .setName('ask')
  .setDescription('Ask the AI')

async function execute(interaction) {
    interaction.reply('Reply');
}

export { data, execute };
```


In order to use the Open AI Api we need to import it. We also need to import the API key. An API key is a password for the API so it knows we (the user) are allowed to access it.

```js
import OpenAI from "openai";

import config from '../../config.json' with { type: "json" };
const { aiApiKey } = config;
```

We need to create a client. The client is the messenger between the user (us) and the API (OpenAi). 

```js
const client = new OpenAI({ apiKey: aiApiKey });
```

In order to send and receive information from the Open AI API, we need to ask our client to create a response for us. 

Here we need to specify the input and the model type. The input can be anything you want to ask the AI. Open AI has several model type based on the difficulty and type of processing your input requires. Today we will be using gpt-3.5-turbo, this will give us text only responses.

```js
const response = await client.responses.create({
    model: "gpt-3.5-turbo",
    input: "Insert prompt here",
});
```

The client will return us a response object. To access only the response as a string we need to use 
```js 
response.output_text 
```

NOTE
We need to specify await here since the API will take a long time to respond.


Alternatively, we can use a variable to take in input. 
Reminder to insert a variable in a string:
```js
`${my_variable}`
```

TASK:
Create an async function that takes in a string input and returns a response from the Open AI client.

REMINDER
The async keyword allows us to use await inside the function.
```js
async my_function {
    ...
    const x = await other_function()
    ...
    return x;
}
```
To call an async function we need to use the keyword await.

```js
const y = await my_function.
```

TASK
Change interaction.reply() so that it uses the response we receive from the Open Ai client. 

CHECKPOINT
The /ask command responds to the user using the Open Ai API. Everytime you run the command you might get a slightly different response. 

NOTE:
If you send to many requests to the API at once the API might freeze. Wait a few minutes between requests. 

ERROR HANDLING
Sometimes the API might fail (eg. internet down, server down). Often errors will interupt the entire program. We can place our code in a try-catch block to prevent 
our program from being stopped completely. 

HINT
```js
async my_function {
    try {
        const x = await other_function();
        return x;
    } catch {
        console.error('Something went wrong:', error)
        return 'Error occured.';
    }
}
```

