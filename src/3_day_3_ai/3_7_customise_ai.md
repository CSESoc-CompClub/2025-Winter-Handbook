
[PUT THIS ON THE NEXT PAGE]
Right now the AI is not responding to the text you sent in Discord. To take in text input from Discord we need to add another option to the SlashCommandBuilder. 


```js
  .addStringOption((option) =>
    option
      .setName('question')
      .setDescription('The question to ask the AI')
      .setRequired(true)
  )
```
In Discord, this appears as 
<!-- insert screenshot from disc -->

We can access the user input from Discord using a function called getString. Place this in the execute() function.

```js
const prompt = interaction.options.getString('question');
```

TASK:
Use the input from Discord to change the prompt given to the AI client.

CHECKPOINT:
The /ask command should now respond to the text you send in discord. 


In the next part, we will show you how to give the AI prompts more specific instructions. 







