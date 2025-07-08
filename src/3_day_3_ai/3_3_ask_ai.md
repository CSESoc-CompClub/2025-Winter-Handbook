# Task 1: Calling Open AI API

The API we are using today is OpenAi. 
To use the API we first need to import it. 

C
```js 
import { GoogleGenAI } from "@google/genai"; 
```

> [!NOTE] Remember to use async and await 
 <!-- WE NEED TO IMPORT THE GOOGLE GEMINI API -->

<!-- 

const ai = new GoogleGenAI({}); INSTANTIATE A NEW AI OBJ

async function main() {
  const response = await ai.models.generateContent({
    model: "gemini-2.5-flash",
    contents: "Explain how AI works in a few words",
  });
  console.log(response.text);
}

await main(); -->