# Azure AI Foundry Chat App

A Python-based chat application built using Azure AI Foundry and the OpenAI Python SDK.

This project follows the Microsoft Learn **Create a Generative AI Chat App** lab and is being developed incrementally to demonstrate modern AI application development with Azure AI Foundry.

---

# Current Status

**Commit 5 – Responses API**

Completed:

* Cloned the Microsoft Learn repository.
* Configured the Python development environment.
* Created a virtual environment.
* Installed project dependencies.
* Configured the application environment.
* Initialized the Azure OpenAI client.
* Implemented Microsoft Entra ID authentication.
* Implemented the Chat Completions API.
* Migrated the application to the Responses API.
* Successfully authenticated using Azure CLI.
* Verified communication with a deployed GPT model.
* Tested the application using the Responses API.

The application now uses the newer Responses API, which provides a simpler interface for interacting with GPT models. Conversation history is not yet maintained between requests and will be implemented in the next stage.

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

## Create a virtual environment

```bash
python -m venv .venv
```

## Activate the virtual environment

Windows

```bash
.venv\Scripts\activate
```

## Install dependencies

```bash
pip install -r python/chat-app/requirements.txt
```

## Configure the application

Create a `.env` file inside `python/chat-app` using `.env.example`.

Configure:

* Azure OpenAI Endpoint
* Model Deployment Name

## Authenticate with Azure

```bash
az login
```

## Run the application

```bash
python chat-app.py
```

---

# Features Implemented

* Azure authentication using Microsoft Entra ID
* Azure OpenAI client initialization
* Responses API integration
* Interactive command-line chat interface
* GPT model response generation

---

# Upcoming Improvements

* Maintain conversation history
* Stream AI responses
* Add asynchronous implementation
* Final project documentation

---

# Learning Outcomes

This project demonstrates practical experience with:

* Azure AI Foundry
* OpenAI Python SDK
* Microsoft Entra ID authentication
* Responses API
* Python virtual environments
* Command-line AI applications

---

# Acknowledgements

This project is based on the Microsoft Learn Azure AI Foundry lab and is being developed as part of my AI Engineering learning journey.
