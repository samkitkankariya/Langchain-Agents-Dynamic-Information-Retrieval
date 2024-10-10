# 🤖 Langchain Agents - Dynamic Information Retrieval

## Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Components](#components)
   - [Tools](#tools)
   - [Agents](#agents)
   - [LLMs](#llms)
6. [Examples](#examples)
7. [Acknowledgments](#acknowledgments)

## Introduction

Welcome to Langchain Agents - Dynamic Information Retrieval, a cutting-edge project that demonstrates the power and versatility of LangChain tools and agents. This project showcases how Large Language Models (LLMs) can interact with various external data sources and perform complex tasks using a combination of natural language processing and specialized tools.

This project is designed to help developers, researchers, and AI enthusiasts understand and experiment with the capabilities of LangChain's ecosystem. By providing a comprehensive set of examples and implementations, it serves as both a learning resource and a foundation for building advanced AI applications.

## Features

- 🔧 Integration of multiple LangChain tools
- 🧠 Implementation of OpenAI's GPT models
- 🌐 Web scraping and information retrieval
- 📚 Access to scientific papers through arXiv
- 🔍 Google Search integration
- 🛠️ Custom tool creation and integration
- 🤖 Agent-based task execution
- 🔄 Dynamic prompt engineering

## Installation

To get started with this project, follow these steps:

```bash
# Clone the repository
git clone https://github.com/yourusername/langchain-agents-dynamic-info-retrieval.git

# Navigate to the project directory
cd langchain-agents-dynamic-info-retrieval

# Create a virtual environment
python -m venv venv

# Activate the virtual environment
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`

# Install the required packages
pip install -r requirements.txt

# Set up your environment variables
cp .env.example .env
# Edit the .env file with your API keys and other configurations
```

Make sure you have Python 3.7+ installed on your system.

## Usage

To run the Langchain Agents notebook:

1. Start Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

2. Open the `Agents_Websites_Google_Search_Wiki.ipynb` file.

3. Run the cells in order to explore the different components and functionalities.

## Components

### Tools

This project integrates several powerful tools to enhance the capabilities of language models:

1. **Web Retriever**: A custom tool that scrapes and retrieves information from specified websites.
2. **arXiv Tool**: Allows the agent to search and fetch scientific papers from the arXiv repository.
3. **Google Search**: Integrates Google's search functionality to find recent and relevant information.
4. **Wikipedia**: Enables the agent to query and extract information from Wikipedia.

Each tool is designed to extend the knowledge and capabilities of the base language model, allowing it to access up-to-date information and perform specialized tasks.

### Agents

The project demonstrates the use of OpenAI's function calling agent, which can:

- Decide which tools to use based on the given task
- Execute tools in a sequential or parallel manner
- Interpret tool outputs and decide on next steps
- Combine information from multiple sources to provide comprehensive answers

### LLMs

This project primarily uses OpenAI's GPT models, specifically:

- GPT-3.5-turbo: For general conversational tasks and tool usage
- GPT-4 (optional): For more complex reasoning and advanced capabilities

## Examples

Here are some examples of what you can do with this project:

1. **Multi-source Research**:
   ```python
   query = "What are the latest advancements in renewable energy technologies?"
   result = agent.run(query)
   print(result)
   ```

2. **Fact-checking and Verification**:
   ```python
   query = "What is the current population of Tokyo? Verify this information from multiple sources."
   result = agent.run(query)
   print(result)
   ```

3. **Comparative Analysis**:
   ```python
   query = "Compare the economic policies of the USA and China in the last 5 years."
   result = agent.run(query)
   print(result)
   ```

## Acknowledgments

- [LangChain](https://github.com/hwchase17/langchain) for providing the foundational tools and frameworks
- OpenAI for their powerful language models
- The open-source community for their invaluable contributions to the AI ecosystem
