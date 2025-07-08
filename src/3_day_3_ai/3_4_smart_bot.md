# Task 4: Creating a SmartBot

Now we want to be able to call the Open Ai using our discord bot. Here we will implement a new slash command: /ask.

Create a new file called ai.js in the commands/utilities folder. 
<!-- insert screenshot of files -->

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

In Discord, these slash commands can take in multiple inputs. These are known as options. 

```js
  .addStringOption((option) =>
    option
      .setName('question')
      .setDescription('The question to ask the AI')
      .setRequired(true)
  );
```


In order to use the Open AI Api we need to import it. We also need to import the API key. An API key is a password for the API so it knows we (the user) are allowed to access it.

```js
import OpenAI from "openai";

import config from '../../config.json' with { type: "json" };
const { aiApiKey } = config;
```

We need to create a client. The client is the messenger between the user and the API. 

```js
const client = new OpenAI({ apiKey: aiApiKey });
```

TASK:
Write an async function that asks the Open Ai client to create a response. 

HINT:
look at previous exercise



