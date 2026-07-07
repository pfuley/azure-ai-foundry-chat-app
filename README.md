# Azure AI Foundry Chat App

A Python-based chat application built as part of the Microsoft Learn **Create a Generative AI Chat App** lab using Azure AI Foundry.

This project demonstrates how to build a conversational AI application with the OpenAI Python SDK and Azure AI Foundry. The application will be developed incrementally across multiple commits, with each commit introducing a new feature or concept.

## Current Status

Commit 3 – Azure OpenAI Client Initialization

Completed:

Cloned the Microsoft Learn repository.
Set up the Python development environment.
Created a Python virtual environment.
Installed the required project dependencies.
Configured the application environment.
Added the Azure OpenAI SDK and Azure Identity imports.
Initialized the Azure OpenAI client using Microsoft Entra ID authentication.

The application is now configured to authenticate with Azure AI Foundry. In the next commit, the chat application will send prompts to the deployed model and display AI-generated responses.

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

## Configuration

Create a `.env` file inside the `python/chat-app` directory by copying the values from `.env.example`.

Update the following settings with your Azure AI Foundry configuration:

* **AZURE_OPENAI_ENDPOINT** – The Azure OpenAI endpoint from your Azure AI Foundry project.
* **MODEL_DEPLOYMENT** – The deployment name of your GPT model.

Example:

```text
AZURE_OPENAI_ENDPOINT=https://your-resource.openai.azure.com/openai/v1/
MODEL_DEPLOYMENT=gpt-5.2
```

The `.env` file contains project-specific configuration and should never be committed to source control.

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
