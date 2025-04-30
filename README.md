## What Is LangChain?

LangChain is an open-source framework designed to help developers build applications powered by LLMs. It provides tools to structure LLM interactions, manage memory, integrate APIs, and create complex workflows.

## Benefits of LangChain

- Simplifies handling prompts and responses
- Supports multiple LLM providers (OpenAI, Hugging Face, Anthropic, etc.)
- Enables memory, retrieval, and chaining multiple AI calls
- Supports building chatbots, agents, and AI-powered apps

## Why Langchain Framework?

Large language models (LLMs) like OpenAI’s GPT-4 and Hugging Face models are powerful, but using them effectively in applications requires more than just calling an API. LangChain is a framework that simplifies working with LLMs, enabling developers to create advanced AI applications with ease.

## NOTES

# 🧠 LangChain: Retrieval Chain & Document Chain Explained

This guide explains two key LangChain components used to build RAG (Retrieval-Augmented Generation) systems: the **Document Chain** and the **Retrieval Chain**, using `create_stuff_documents_chain` and `ChatPromptTemplate`.

---

## 📘 What Is a Document Chain?

A **Document Chain** is responsible for:

- Taking retrieved documents (chunks).
- Merging or formatting them into a single prompt.
- Sending that prompt to the LLM for answering.

### 🔧 Example: Using `create_stuff_documents_chain`

```python
from langchain.chains.combine_documents import create_stuff_documents_chain
from langchain_core.prompts import ChatPromptTemplate



## Create and Setup `venv` in langchain

#### 1. create a `venv` using conda

```

conda create -p venv python==3.11 -y

```

#### 2. create a `requirements.txt`

- langchain
- ipykernel

#### 3. install your packages in `requirements.txt`

```

pip install -r requirements.txt

```

#### 4. confirm if a package is installed

```

pip list | findstr "name_of_package"

```

#### 5. activate the `conda environment`

```

conda activate venv

```

### LLM FAQs

![one-shot-prompting-explained](assets/one-shot-prompting-explained.png)
```
