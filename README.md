# Azure AI Foundry Chat App

A Python-based chat application built using Azure AI Foundry and the OpenAI Python SDK.

This project follows the Microsoft Learn **Create a Generative AI Chat App** lab and is being developed incrementally to demonstrate the complete development process of building a conversational AI application.

---

# Current Status

**Commit 4 – Chat Completions API**

Completed:

* Cloned the Microsoft Learn repository.
* Configured the Python development environment.
* Created a virtual environment.
* Installed all required dependencies.
* Configured the application using environment variables.
* Initialized the Azure OpenAI client.
* Implemented authentication using Microsoft Entra ID.
* Implemented the Chat Completions API.
* Authenticated successfully using Azure CLI (`az login`).
* Successfully connected to the deployed GPT model in Azure AI Foundry.
* Verified end-to-end communication by asking the model about the ELIZA chatbot.
* Successfully terminated the application using the `quit` command.

The application is now capable of sending prompts to a deployed GPT model and displaying AI-generated responses.

---

# Technologies

* Python 3.13
* Azure AI Foundry
* OpenAI Python SDK
* Azure Identity
* Azure CLI
* Visual Studio Code
* Git

---

# Project Structure

```text
foundry-chat/
├── python/
│   └── chat-app/
│       ├── chat-app.py
│       ├── chat-async.py
│       ├── requirements.txt
│       └── .env.example
├── .gitignore
└── README.md
```

---

# Getting Started

## 1. Create a virtual environment

```bash
python -m venv .venv
```

## 2. Activate the virtual environment

Windows

```bash
.venv\Scripts\activate
```

## 3. Install dependencies

```bash
pip install -r python/chat-app/requirements.txt
```

## 4. Configure the application

Create a `.env` file inside `python/chat-app` using `.env.example`.

Configure:

* Azure OpenAI Endpoint
* Model Deployment Name

## 5. Authenticate with Azure

```bash
az login
```

## 6. Run the application

```bash
python chat-app.py
```

---

# Features Implemented

* Azure authentication using Microsoft Entra ID
* Azure OpenAI client initialization
* Chat Completions API integration
* Interactive command-line chat interface
* GPT model response generation

---

# Development Roadmap

* Migrate to the Responses API
* Add conversation history
* Implement streaming responses
* Build an asynchronous chat client
* Improve documentation
* Final project polish

---

# Learning Outcomes

This project demonstrates practical experience with:

* Azure AI Foundry
* Azure authentication
* OpenAI Python SDK
* Chat Completions API
* Python virtual environments
* Building command-line AI applications

---

# Acknowledgements

This project is based on the Microsoft Learn Azure AI Foundry lab and is being developed as part of my AI Engineering learning journey.
