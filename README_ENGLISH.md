# Blackbeard Extension

[日本語版 README はこちら](README.md) | [中文版 README 在这里](README_CHINESE.md)

## Overview

Blackbeard is a sample project for GitHub Copilot Extension. This agent interacts with users as a pirate character and leverages Copilot's LLM API. It is provided as a basic example for learning how to develop GitHub Copilot Extensions.

The main functionality and logic are implemented in the index.js file.

## Features

- Responds to messages as a pirate-like character
- Uses GitHub Copilot's LLM API
- Implements specific behaviors through customized system prompts
- Sample implementation showing the basic structure of Copilot Extensions

## Development Environment Setup

### Prerequisites

- Node.js (LTS) must be installed
- npm must be installed

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

## How to Switch from GitHub Model Endpoint to OpenAI Model Endpoint
To change from GitHub Copilot's model endpoint to OpenAI's model endpoint, replace the files in the `openai-ver` folder with the respective `index.js` files.

- index.js: Basic sample agent scenario
- advance.js: Agent scenario with weather forecast function added
- advance-2.js: Agent scenario with weather forecast function and ability to respond to user self-introductions

Also, rename `.env.sample` to `.env` and set the necessary environment variables.

```bash
cp .env.sample .env
```

The `.env` file needs to have the following environment variables set:

```
# .env
API_KEY="sk-xxxxxxxxxxxxxxxxx" ← Replace with your OpenAI API key
```

## Related Documentation

For detailed information, please refer to the following official documentation:

- [Using Copilot Extensions](https://docs.github.com/en/copilot/using-github-copilot/using-extensions-to-integrate-external-tools-with-copilot-chat)
- [About building Copilot Extensions](https://docs.github.com/en/copilot/building-copilot-extensions/about-building-copilot-extensions)
- [Set up process](https://docs.github.com/en/copilot/building-copilot-extensions/setting-up-copilot-extensions)
- [Communicating with the Copilot platform](https://docs.github.com/en/copilot/building-copilot-extensions/building-a-copilot-agent-for-your-copilot-extension/configuring-your-copilot-agent-to-communicate-with-the-copilot-platform)
- [Communicating with GitHub](https://docs.github.com/en/copilot/building-copilot-extensions/building-a-copilot-agent-for-your-copilot-extension/configuring-your-copilot-agent-to-communicate-with-github)

## Usage

Please use this sample as a reference when developing your own Copilot Extension. You can change the character, add new features, or customize it for specific use cases.