# Blackbeard Extension

[日本語版 README はこちら](README.md) | [English README is here](README_ENGLISH.md)

## 概述

Blackbeard 是 GitHub Copilot Extension 的示例项目。这个代理以海盗角色与用户互动，并利用 Copilot 的 LLM API。它作为学习如何开发 GitHub Copilot Extensions 的基础示例提供。

主要功能和逻辑在 index.js 文件中实现。

## 特性

- 以海盗角色回应消息
- 使用 GitHub Copilot 的 LLM API
- 通过自定义系统提示实现特定行为
- 展示 Copilot Extensions 基本结构的示例实现

## 开发环境设置

### 前提条件

- 必须安装 Node.js (LTS)
- 必须安装 npm

### 安装步骤

安装依赖项：

```bash
npm install
```

### 运行方法

标准模式运行：

```bash
npm start
```

开发模式运行（监视开发过程中的更改）：

```bash
npm run dev
```

## 如何从 GitHub 模型端点切换到 OpenAI 模型端点
要从 GitHub Copilot 的模型端点更改为 OpenAI 的模型端点，请将 `openai-ver` 文件夹中的文件分别替换为相应的 `index.js` 文件。

- index.js: 基础示例代理场景
- advance.js: 添加了天气预报功能的代理场景
- advance-2.js: 添加了天气预报功能并能够回应用户自我介绍的代理场景

此外，将 `.env.sample` 重命名为 `.env` 并设置必要的环境变量。

```bash
cp .env.sample .env
```

`.env` 文件需要设置以下环境变量：

```
# .env
API_KEY="sk-xxxxxxxxxxxxxxxxx" ← 替换为您的 OpenAI API 密钥
```

## 相关文档

详细信息请参考以下官方文档：

- [Using Copilot Extensions](https://docs.github.com/en/copilot/using-github-copilot/using-extensions-to-integrate-external-tools-with-copilot-chat)
- [About building Copilot Extensions](https://docs.github.com/en/copilot/building-copilot-extensions/about-building-copilot-extensions)
- [Set up process](https://docs.github.com/en/copilot/building-copilot-extensions/setting-up-copilot-extensions)
- [Communicating with the Copilot platform](https://docs.github.com/en/copilot/building-copilot-extensions/building-a-copilot-agent-for-your-copilot-extension/configuring-your-copilot-agent-to-communicate-with-the-copilot-platform)
- [Communicating with GitHub](https://docs.github.com/en/copilot/building-copilot-extensions/building-a-copilot-agent-for-your-copilot-extension/configuring-your-copilot-agent-to-communicate-with-github)

## 使用方法

请将此示例作为开发您自己的 Copilot Extension 时的参考。您可以更改角色、添加新功能或为特定用例进行自定义。