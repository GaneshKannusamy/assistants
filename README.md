
<p align="center">
<img width="600" alt="assistants" src="https://github.com/stellar-amenities/assistants/assets/25003283/d160b5b6-450b-469f-ba6b-929de2e87bcf">
  <h1 align="center">⭐️ Open Source Assistants API</h1>
  <h2 align="center">Build Powerful AI Assistants In-House, On Your Terms</h2>
  <h4 align="center">75% Cheaper & 23x Faster Assistants. Same API/SDK.</h4>
  <p align="center">
    <a href="https://discord.gg/XMetBW3zCG"><img alt="Join Discord" src="https://img.shields.io/discord/1066022656845025310?color=blue&style=for-the-badge"></a>
    <hr />
    <a href="https://cal.com/louis030195/unleash-llms">📞 Need Support? We're here for you.</a>
    <br />
    <a href="https://link.excalidraw.com/readonly/YSE7DNzB2LmEPfVdCqq3">🖼️ How it Works – Visual Guide</a>
    <br />
    <a href="https://github.com/stellar-amenities/assistants/issues/new?assignees=&labels=enhancement">✨ Suggest a Feature</a>
    <br />
    <a href="https://github.com/stellar-amenities/assistants/issues/new?assignees=&labels=bug">❤️‍🩹 Found a Bug? Let us know.</a>
  </p>
</p>


# Quickstart

```diff
// Import the essentials
const assistant = await openai.beta.assistants.create({
  // Define your assistant's purpose
  instructions: "You are a weather bot. Fetch and display weather data.",
  // Choose your model
-  model: "gpt4",
+  model: "OpenSourceModel/your-model-v1",
  // Set up the tools for your assistant
  tools: [{
    "type": "function",
    "function": {
      "name": "getCurrentWeather",
      "description": "Fetch weather for a location",
      "parameters": {
        "location": {"type": "string", "description": "City and state, e.g., San Francisco, CA"},
        "unit": {"type": "string"}
      },
      "required": ["location"]
    }
  }]
});
```

[👉 Get started on your machine right now.](./examples/hello-world-intel-neural-chat-nodejs-function-calling/README.md)

## Why Open Source Assistants API?
- **Full Control**: Own your data, your models, and your destiny.
- **No Hidden Costs**: Absolutely free. Seriously, no strings attached.
- **Customizable**: Tailor the AI to your specific needs and use cases.
- **Offline Capabilities**: Perfect for edge cases or internet-free zones.
- **OpenAI Compatibility**: Love OpenAI's API? We play nice with that too.
- **Simplicity**: Easy setup, no steep learning curve.

## What's Cooking? – Latest News

- [2023/08/12] 🔥 New example: Open source LLM with function calling. [Learn more](./examples/hello-world-intel-neural-chat-nodejs-function-calling/README.md).
- [2023/29/11] 🔥 New example: Using mistral-7b, an open source LLM. [Check it out](./examples/hello-world-mistral-curl/README.md).

## Key Features
- [ ] **Code Interpreter**: Runs Python code in a sandboxed environment.
  - [ ] Anthropic
  - [ ] Open source LLMs (We're working on it!)
- [x] **Knowledge Retrieval**: Retrieves external knowledge or documents.
  - [x] Anthropic
  - [x] Open source LLMs
- [x] **Function Calling**: Defines and executes custom functions.
  - [x] Anthropic
  - [x] Open source LLMs
- [x] **File Handling**: Supports a range of file formats.
  - [x] pdf, text files
  - [ ] images, videos, etc. (We're working on it!)

## What can you build with Assistants?

- [Perplexity for Astronauts: Stellar Amenities uses Assistants to let the LLM automatically find the right information on the spacecraft to help Astronauts](https://ai.stellaramenities.space)

## Join the Movement
- **For Developers**: We've got the docs, tools, and a community ready to help you build what's next.
- **For Innovators**: Looking for an edge in AI? Here's where you leapfrog the competition.
- **For the Visionaries**: Dreamt of a custom AI assistant? Let's make it a reality.

Ready to build your AI assistant with freedom? [Start here.](./examples/hello-world-intel-neural-chat-nodejs-function-calling/README.md)

## Deployment

Please follow [this documentation](https://github.com/stellar-amenities/assistants/blob/main/ee/k8s/README.md).

## FAQ

<details>
<summary>What's the difference with LangChain?</summary>
LangChain offers detailed control over AI conversations, while OpenAI's Assistants API simplifies the process, managing conversation history, data/vector store, and tool switching for you.
</details>

<details>
<summary>Are you related to OpenAI?</summary>
No.
</details>

<details>
<summary>I don't use Assistants API. Can I use this?</summary>
We recommend switching to the Assistants API for a more streamlined experience, allowing you to focus more on your product than on infrastructure.
</details>

<details>
<summary>Does the Assistants API support audio and images?</summary>
Images soon, working on it.
Audio in a few weeks.
</details>
