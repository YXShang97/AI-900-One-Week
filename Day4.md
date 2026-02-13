# AI-900 Study Notes - Day 4 - Generative AI

**Generative AI** is the **ability to generate content based on a language model**, which has been trained with huge volumes of data, often documents from the Internet or other public sources of information.

**Large language models (LLMs)** are trained on large volumes of data (TBs) and are very powerful but more costly to train and use. LLMs are trained to **generate completions based on prompts**.

- **Tokenization**: The process of **breaking down text into smaller units** called tokens, which can be words, subwords, or characters.
- **Embeddings**: The result of **mapping tokens to vectors** in a continuous vector space, **capturing semantic meaning**.
- **Attention Mechanism**: Helps models **focus on relevant parts of the input** but is not involved in the initial breaking down of text.
- **System Prompt**: Sets the **behavior** and **tone of the model**, and any **constraints** it should adhere to.

### Azure OpenAI Service

A managed service that provides access to generative models (GPT-3.5, GPT-4, DALL-E).

- **GPT-3.5**: A large language model developed by OpenAI, known for its ability to **generate human-like text based on prompts**. It was widely used in applications requiring natural language understanding and generation, such as straightforward text generation (e.g., Q&A) or tasks not requiring complex reasoning.
- **DALL-E**: An AI model developed by **OpenAI** that **generates images from textual descriptions**. It enables users to create unique visuals by simply describing them in words (text-to-image).

### AI Foundry

Provides an enterprise-grade environment to develop, test, and deploy generative AI solutions. It acts as **Azure’s hub for generative AI and AI Services** to pick a model, fine-tune, build apps, and monitor usage.

- **Model Catalog**: A **centralized repository of foundation models** from Microsoft, OpenAI, and other AI leaders that allows you to **discover, compare, and select** models for generative AI tasks.

### Microsoft Purview

Assess and **manage compliance for your AI apps**. It translates AI regulations, such as the EU AI Act, into actionable suggestions that you can implement in Microsoft Foundry to run your AI evaluations.

### Safety System

A layer that includes platform-level configurations and capabilities to help **mitigate harm**. For example, the Azure OpenAI service includes support for **content filters that apply criteria to suppress prompts** and responses based on the classification of content into four severity levels (safe, low, medium, and high) for **four categories of potential harm (hate, sexual, violence, and self-harm)**.

### Copilots

Use **plugins to provide end users with the ability to get help with common tasks** from a generative AI model.
