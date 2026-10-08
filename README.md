# 🧴 AI Skincare Messenger Bot

An AI-powered Messenger chatbot designed for skincare businesses to automate customer support and help customers discover suitable skincare products through natural conversation.

The project combines **n8n, AI Agents, RAG, and Supabase** to create a knowledge-based conversational assistant that answers customer questions using the business's skincare product information.

## 🚀 Project Overview

Customers can interact with the chatbot through Messenger and ask questions about skincare products, ingredients, usage, and available options.

Instead of relying only on the LLM's general knowledge, the chatbot uses a **Retrieval-Augmented Generation (RAG)** approach to retrieve relevant information from the skincare product knowledge base before generating a response.

This helps the chatbot provide responses based on the business's actual product data.

## ✨ Features

- 💬 AI-powered Messenger conversations
- 🧴 Skincare product recommendations based on customer needs
- 🔎 RAG-based product information retrieval
- 🤖 AI Agent for understanding and processing customer requests
- 📚 Knowledge base for skincare products
- 🗄️ Supabase for storing and retrieving vectorized information
- 🔄 n8n workflow automation
- 🔗 Integration between Messenger, AI models, n8n, and Supabase
- ⚡ Automated customer support

## 🏗️ Architecture

```text
Customer
   │
   ▼
Messenger
   │
   ▼
n8n Workflow
   │
   ▼
AI Agent
   │
   ├──────────────► Supabase Vector Database
   │                       │
   │                       ▼
   │                Relevant Product Data
   │
   ▼
LLM
   │
   ▼
AI-generated Response
   │
   ▼
Messenger
   │
   ▼
Customer
```

## 🔧 Technologies Used

- **n8n** — Workflow automation
- **AI Agent** — Customer request processing and decision making
- **RAG (Retrieval-Augmented Generation)** — Knowledge-based responses
- **Supabase** — Database and vector search
- **LLM API** — Natural language understanding and response generation
- **Messenger API** — Customer communication

## 🧠 How It Works

1. A customer sends a message through Messenger.
2. The message is received by the n8n workflow.
3. The AI Agent analyzes the customer's request.
4. Relevant information is retrieved from the skincare knowledge base using RAG.
5. Supabase performs the required data/vector retrieval.
6. The retrieved information is provided to the LLM as context.
7. The LLM generates a natural-language response.
8. The response is sent back to the customer through Messenger.

## 📚 Example Use Cases

The chatbot can answer questions such as:

- "Which moisturizer is suitable for dry skin?"
- "What ingredients are in this product?"
- "How should I use this serum?"
- "Do you have a cleanser for oily skin?"
- "What products are available for sensitive skin?"

## 🎯 Business Value

This chatbot can help skincare businesses:

- Automate repetitive customer questions
- Provide faster responses
- Make product information easier to access
- Reduce manual customer-support workload
- Provide 24/7 automated assistance
- Improve the customer product-discovery experience

## 🔐 Security

No private API keys, access tokens, customer information, or sensitive credentials are included in this repository.

All credentials are stored securely in the relevant n8n credentials/environment configuration.

## 📸 Demo

Add screenshots or a short video demonstrating the Messenger conversation and n8n workflow here.

## 👩‍💻 Author

**Mai**

AI Automation & n8n Developer

Specializing in:

- AI Automation
- n8n Workflows
- AI Agents
- RAG Systems
- LLM Integrations
- API Integrations
- Chatbots
