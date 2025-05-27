# Blackbeard Extension

*[English version here](README_EN.md)*

## 概要

Blackbeard は、GitHub Copilot Extension のサンプルプロジェクトです。このエージェントは海賊のキャラクターとしてユーザーとやり取りし、Copilot の LLM API を活用しています。GitHub Copilot Extension の開発方法を学ぶための基本的な例として提供されています。

主要な機能やロジックは index.js ファイルに実装されています。

## 特徴

- 海賊のようなキャラクターとしてメッセージに応答
- GitHub Copilot の LLM API を使用
- カスタマイズされたシステムプロンプトによる特定の動作の実装
- Copilot Extension の基本構造を示すサンプル実装

## 開発環境のセットアップ

### 前提条件

- Node.js (LTS) がインストールされていること
- npm がインストールされていること

### インストール手順

依存関係をインストールします：

```bash
npm install
```

### 実行方法

標準モードで実行：

```bash
npm start
```

開発中に変更を監視する開発モードで実行：

```bash
npm run dev
```

## GitHub のモデルのエンドポイントから OpenAI のモデルのエンドポイントに変更する方法
GitHub Copilot のモデルのエンドポイントを OpenAI のモデルのエンドポイントに変更するには、`openai-ver`フォルダの中にあるファイルをそれぞれ `index.js`に置き換えます。

- index.js: 基本的なサンプルエージェントのシナリオ
- advance.js: 天気予報の関数を追加したエージェントのシナリオ
- advance-2.js: 天気予報の関数を追加し、ユーザーの自己紹介にも回答できるようにしたエージェントのシナリオ

また、`.env.sample`を `.env`にリネームし、必要な環境変数を設定してください。

```bash
cp .env.sample .env
```

`.env`ファイルには、以下の環境変数を設定する必要があります：

```
# .env
API_KEY="sk-xxxxxxxxxxxxxxxxx" ← OpenAI の API キーに置き換えてください
```

## 関連ドキュメント

詳細な情報については、以下の公式ドキュメントを参照してください：

- [Using Copilot Extensions](https://docs.github.com/en/copilot/using-github-copilot/using-extensions-to-integrate-external-tools-with-copilot-chat)
- [About building Copilot Extensions](https://docs.github.com/en/copilot/building-copilot-extensions/about-building-copilot-extensions)
- [Set up process](https://docs.github.com/en/copilot/building-copilot-extensions/setting-up-copilot-extensions)
- [Communicating with the Copilot platform](https://docs.github.com/en/copilot/building-copilot-extensions/building-a-copilot-agent-for-your-copilot-extension/configuring-your-copilot-agent-to-communicate-with-the-copilot-platform)
- [Communicating with GitHub](https://docs.github.com/en/copilot/building-copilot-extensions/building-a-copilot-agent-for-your-copilot-extension/configuring-your-copilot-agent-to-communicate-with-github)

## 活用方法

このサンプルをベースに独自の Copilot Extension を開発する際の参考にご利用ください。キャラクターの変更、新機能の追加、または特定のユースケースに合わせたカスタマイズが可能です。
