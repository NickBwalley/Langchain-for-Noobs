#### What Is LangChain?

LangChain is an open-source framework designed to help developers build applications powered by LLMs. It provides tools to structure LLM interactions, manage memory, integrate APIs, and create complex workflows.

#### Benefits of LangChain

- Simplifies handling prompts and responses
- Supports multiple LLM providers (OpenAI, Hugging Face, Anthropic, etc.)
- Enables memory, retrieval, and chaining multiple AI calls
- Supports building chatbots, agents, and AI-powered apps

#### Why Langchain Framework?

Large language models (LLMs) like OpenAI’s GPT-4 and Hugging Face models are powerful, but using them effectively in applications requires more than just calling an API. LangChain is a framework that simplifies working with LLMs, enabling developers to create advanced AI applications with ease.

#### Explanations.

- `from langchain_openai import ChatOpenAI()`. This imports the ChatOpenAI class from the langchain_openai package and allows to use OpenAI’s GPT-based models for conversational AI.
- `ChatOpenAI()`. This initializes the GPT model.
- `model ="gpt-3.5-turbo"`. As Open AI has several models to use, we have to pass the model that we want to use for prompt response. However, by default, Open AI uses the text-davinci-003 model.
  temperaure=0.5. ChatOpenAI is initialized with a temperature of 0.5. Temperature controls randomness in the response:
- 0.0: Deterministic (always returns the same output for the same input).
- 0.7: More creative/random responses.
- 1.0: Highly random and unpredictable responses.
- Since temperature = 0.5, it balances between creativity and reliability.
- `prompt = "What is LangChain?"`. Here, we are defining the prompt, which is coming from LangChain and will be sent to the ChatOpenAI model for processing.
- `llm.invoke(prompt)`. This sends the prompt to the given LLM and gets the response.
