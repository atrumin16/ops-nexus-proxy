# ops-nexus-proxy

A highly performant, serverless AI gateway and ChatGPT-inspired UI client designed for systems automation, documentation generation, and deterministic technical tasks. 

This project operates as a secure, stateless proxy that routes client requests to high-efficiency open-source models without exposing private API credentials on the frontend.

---

## 🚀 Features

* **ChatGPT-Style Interface:** A pixel-perfect, dark-mode web UI built with Tailwind CSS, featuring a persistent sidebar, minimalist message layouts, and monospaced blocks for technical scripts.
* **Advanced JS Engine:** Implements client-side markdown parsing for code blocks, real-time typewriter effect (simulated streaming), and session persistence via browser `localStorage`.
* **Serverless Proxy Architecture:** Powered by Cloudflare Workers, keeping your backend footprint completely zero-cost and lightweight.
* **Qwen Engine Integration:** Utilizes `qwen-3-32b` via Groq for fast, low-latency, and highly precise technical text and script generation.
* **Production-Ready Security:** API credentials are fully isolated on the server side using Cloudflare Environment Secrets, preventing client-side leaks or API abuse.

---

## 📂 Project Structure

```text
├── .gitignore          # Prevents sensitive local environment files from being tracked
├── LICENSE             # MIT License file
├── README.md           # Project documentation
├── index.html          # High-fidelity ChatGPT clone frontend with advanced JS
├── worker.js           # Serverless Cloudflare Worker (Groq API Proxy)
└── wrangler.toml       # Cloudflare deployment and public variables configuration
