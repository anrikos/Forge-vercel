# Prompt Market Analyzer 🛒🤖

Language / Язык: **English** | [Русский (Russian)](README.ru.md)

---

An intelligent web application designed to automate grocery price analysis across various retail chains. The service generates well-structured, detailed prompts for AI, supports hands-free voice input, and communicates directly with the Google Gemini API via Vercel Edge Serverless functions.

**Live Demo:** [forge-vercel-hazel.vercel.app](https://vercel.app)

## ✨ Features
* **Voice-to-Text Input:** Dictate grocery lists and store names naturally using your microphone (Web Speech API).
* **Direct Gemini API Integration:** Execute market analysis requests straight from the dashboard through a secure Vercel Edge proxy.
* **Privacy-First:** Your Gemini API key is stored securely on your own device inside the browser's `localStorage`.
* **Multi-Platform Support:** Instantly export generated prompts and launch them in ChatGPT, Microsoft Copilot, or Google AI with a single click.
* **Modern Glassmorphic UI:** A futuristic, responsive dark-themed interface built with smooth blur effects and modern CSS variables.

## 🛠 Project Structure
The project is tailored for instant deployment on the Vercel platform without requiring any local build steps or external package installations:
* **`index.html`** – Frontend client app written in vanilla JavaScript, CSS variables, and FontAwesome icons.
* **`api/`** – Node.js Serverless Functions that act as an API proxy to pipe requests securely.
* **`vercel.json`** – Vercel routing configuration and edge deployment rules.

```text
├── api/             # API Endpoints (Node.js Serverless Functions)
├── index.html       # Web Interface (Frontend client)
└── vercel.json      # Vercel Deployment Configuration
```

## 🚀 Deployment
1. Connect this GitHub repository to your Vercel Account.
2. Every `git push` into the `main` branch will trigger an automated production deployment on Vercel.

## 🚀 Развертывание (Deployment)

Приложение полностью адаптировано под автоматический деплой:

1. **Интеграция с GitHub:** Достаточно подключить репозиторий к вашему аккаунту Vercel.
2. **CI/CD:** При каждом `git push` в ветку `main` Vercel самостоятельно разворачивает фронтенд и изолирует бессерверные функции из папки `api/`.
