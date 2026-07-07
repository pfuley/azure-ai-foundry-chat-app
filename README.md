# Azure AI Foundry Chat App

A Python-based chat application built as part of the Microsoft Learn **Create a Generative AI Chat App** lab using Azure AI Foundry.

This project demonstrates how to build a conversational AI application with the OpenAI Python SDK and Azure AI Foundry. The application will be developed incrementally across multiple commits, with each commit introducing a new feature or concept.

## Current Status

**Commit 1 – Initial Project Setup**

This commit establishes the project foundation.

Completed:

* Cloned the Microsoft Learn repository
* Set up the Python development environment
* Created a Python virtual environment
* Installed the required project dependencies
* Prepared the project structure for development

No application functionality has been implemented yet.

## Technology Stack

* Python 3.13
* Azure AI Foundry
* OpenAI Python SDK
* Azure Identity
* Azure CLI
* Visual Studio Code
* Git

## Project Structure

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

## Getting Started

1. Create and activate a Python virtual environment.
2. Install the required dependencies.

```bash
pip install -r python/chat-app/requirements.txt
```

3. Create a `.env` file from `.env.example`.
4. Configure your Azure AI Foundry endpoint and model deployment.
5. Continue implementing the application.

## Development Roadmap

* Configure Azure authentication
* Initialize the OpenAI client
* Implement Chat Completions
* Migrate to the Responses API
* Add conversation history
* Implement streaming responses
* Build an asynchronous chat client
* Finalize project documentation

## Acknowledgements

This project is based on the Microsoft Learn Azure AI Foundry lab and is being developed as a learning project to better understand modern AI application development.
