# Azure AI Foundry Chat App

A Python-based conversational AI application built with **Azure AI Foundry**, the **OpenAI Python SDK**, and **Microsoft Entra ID** authentication.

This project was developed by following the Microsoft Learn **Create a Generative AI Chat App** lab while documenting each major milestone through incremental Git commits. The application demonstrates how to connect a Python application to a GPT model deployed in Azure AI Foundry and progressively introduces modern AI development concepts such as the Responses API, conversation tracking, streaming responses, and asynchronous programming.

---

# Features

* Microsoft Entra ID authentication
* Azure AI Foundry integration
* OpenAI Python SDK
* Chat Completions API implementation
* Responses API implementation
* Conversation tracking using response IDs
* Streaming AI responses
* Asynchronous chat client
* Interactive command-line interface

---

# Technology Stack

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
│       ├── chat-app.py          # Synchronous chat application
│       ├── chat-async.py        # Asynchronous chat application
│       ├── requirements.txt
│       ├── .env.example
│       └── .env                # Local configuration (not committed)
├── .gitignore
└── README.md
```

---

# Getting Started

## Clone the repository

```bash
git clone https://github.com/pfuley/azure-ai-foundry-chat-app.git
```

## Create a virtual environment

```bash
python -m venv .venv
```

## Activate the virtual environment

### Windows

```bash
.venv\Scripts\activate
```

## Install dependencies

```bash
pip install -r python/chat-app/requirements.txt
```

## Configure the application

Create a `.env` file inside `python/chat-app` using `.env.example`.

Configure the following values:

* Azure OpenAI Endpoint
* Model Deployment Name

## Authenticate with Azure

```bash
az login
```

## Run the synchronous application

```bash
python chat-app.py
```

## Run the asynchronous application

```bash
python chat-async.py
```

---

# Project Journey

This repository was developed incrementally to demonstrate the evolution of an AI application.

| Commit | Description                       |
| ------ | --------------------------------- |
| 1      | Initial project setup             |
| 2      | Configure application environment |
| 3      | Initialize Azure OpenAI client    |
| 4      | Implement Chat Completions API    |
| 5      | Migrate to the Responses API      |
| 6      | Add conversation tracking         |
| 7      | Implement streaming responses     |
| 8      | Add asynchronous chat client      |

---

# Concepts Demonstrated

This project demonstrates practical implementation of:

* Azure AI Foundry
* Microsoft Entra ID authentication
* OpenAI Python SDK
* Chat Completions API
* Responses API
* Conversation context management
* Streaming responses
* Asynchronous programming with Python
* Python virtual environments

---

# Example Workflow

1. Authenticate using Azure CLI.
2. Connect to Azure AI Foundry.
3. Send a user prompt.
4. Generate an AI response.
5. Maintain conversation context.
6. Stream responses to the terminal.
7. Continue the conversation or exit.

---

# Future Improvements

This project intentionally leaves room for additional enhancements. Planned improvements include:

* Improved error handling and retry logic
* Logging and diagnostics
* Configuration validation
* Better command-line user experience
* Unit and integration tests
* Docker support
* GitHub Actions CI/CD
* Deployment examples
* Web interface using Flask or FastAPI
* Retrieval-Augmented Generation (RAG)
* Tool calling and AI agents
* Conversation persistence
* Additional Azure AI Foundry capabilities

---

# Learning Outcomes

Building this project provided hands-on experience with:

* Authenticating against Azure services
* Building AI-powered Python applications
* Working with synchronous and asynchronous APIs
* Managing conversational context
* Streaming model responses
* Structuring an AI project for version control and incremental development

---

# Acknowledgements

This project is based on the Microsoft Learn Azure AI Foundry lab and has been adapted as a personal learning project to explore modern AI application development using Python and Azure AI Foundry.
