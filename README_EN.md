# Blackbeard Extension

*[日本語版はこちら](README.md)*

## Overview

Blackbeard is a sample project for GitHub Copilot Extension. This agent interacts with users as a pirate character, utilizing the Copilot LLM API. It is provided as a basic example to learn how to develop GitHub Copilot Extensions.

The main functionality and logic are implemented in the index.js file.

## Features

- Responds to messages as a pirate character
- Uses GitHub Copilot's LLM API
- Implements specific behaviors through customized system prompts
- Sample implementation showing the basic structure of a Copilot Extension

## Development Environment Setup

### Prerequisites

- Node.js (LTS) installed
- npm installed

### Installation Steps

Install dependencies:

```bash
npm install
```

### How to Run

Run in standard mode:

```bash
npm start
```

Run in development mode to watch for changes during development:

```bash
npm run dev
```

## How to Change from GitHub Model Endpoint to OpenAI Model Endpoint
To change the model endpoint from GitHub Copilot to OpenAI, replace the corresponding `index.js` with the files in the `openai-ver` folder.

- index.js: Basic sample agent scenario
- advance.js: Agent scenario with added weather forecast function
- advance-2.js: Agent scenario with added weather forecast function and ability to respond to user self-introductions

Also, rename `.env.sample` to `.env` and set the required environment variables.

```bash
cp .env.sample .env
```

In the `.env` file, you need to set the following environment variables:

```
# .env
API_KEY="sk-xxxxxxxxxxxxxxxxx" ← Replace with your OpenAI API key
```

## Related Documents

For more detailed information, refer to the following official documentation:

- [Using Copilot Extensions](https://docs.github.com/en/copilot/using-github-copilot/using-extensions-to-integrate-external-tools-with-copilot-chat)
- [About building Copilot Extensions](https://docs.github.com/en/copilot/building-copilot-extensions/about-building-copilot-extensions)
- [Set up process](https://docs.github.com/en/copilot/building-copilot-extensions/setting-up-copilot-extensions)
- [Communicating with the Copilot platform](https://docs.github.com/en/copilot/building-copilot-extensions/building-a-copilot-agent-for-your-copilot-extension/configuring-your-copilot-agent-to-communicate-with-the-copilot-platform)
- [Communicating with GitHub](https://docs.github.com/en/copilot/building-copilot-extensions/building-a-copilot-agent-for-your-copilot-extension/configuring-your-copilot-agent-to-communicate-with-github)

## How to Use

Use this sample as a reference when developing your own Copilot Extension. You can change the character, add new features, or customize it for specific use cases.