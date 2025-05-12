# Session 3: Generative AI & Prompting

## AI/Neural Networks/Machine Learning/LLM

In general, what is now called AI (Artificial Intelligence) is an (artificial-) Neural Network based Large Language Model (LLM), which is a type of Machine Learning (ML).

As a very high-level overview, Large Language Models (LLMs) are huge neural networks (having billions to trillions of parameters) trained on vast amounts of text data. They are "trained" to predict the next "word" in a sentence. Therefore, they pick up the surface-level patterns of a language in the beginning, and first, they usually output good-sounding jibberish. However, with enough training, parameters and data, their answers become more and more meaningful, and seemingly pick up deeper, meaning-related patterns of the language. After a certain threshold, they can access, apply and combine information from the training data.

However, without extra effort, they are not reliable. A common feature of these models is hallucination, i.e. they tend to generate good-sounding parts which would fit well into the context, but are absolutely not true.

Another problematic feature of these systems is their "intelligence" (which is itself a not well-defined term). LLMs are surprisingly useful in various tasks, but to predict their behaviour, it is not always helpful to reason based on "human-like intelligence". To some extent, they can "roleplay" *as if* they were intelligent, but they do not have a similar motivation and drive system as most humans do. Maybe once we will need to revise our understanding of intelligence, personality, goals and even "consciousness", but for now it seems to be safe to say that these "AI"-s are capable of finding deeper patterns in data, and combine them to produce novel and often accurate answers.

### Popular LLMs

- [ChatGPT](https://chatgpt.com/) - by OpenAI
- [Claude](https://claude.ai/) - by Anthropic
- [Gemini](https://gemini.google.com/app) - by Google DeepMind
- Further LLMs:
    - [Mistral](https://mistral.ai/) - by Mistral (French startup)
    - [Pi](https://pi.ai/) - by Inflection AI
    - [DeepSeek](https://www.deepseek.com/) - by DeepSeek
    - [Meta](https://www.meta.ai/) - by Meta (Facebook)

### Further AI based tools

- [GitHub Copilot](https://github.com/features/copilot) - An AI-powered code completion tool (available for instance in Visual Studio Code).
- [Grammarly](https://www.grammarly.com/) - A writing assistant that uses AI to help you write better.


## Prompt Engineering

### Prompt Engineering Guide

- [Prompt Engineering Guide](https://www.promptingguide.ai/)

### Other Prompt Engineering Guides

- [Cohere](https://docs.cohere.com/v2/docs/crafting-effective-prompts)
- [Google Gemini](https://ai.google.dev/gemini-api/docs/prompting-strategies)
- [Microsoft](https://learn.microsoft.com/en-us/azure/ai-services/openai/concepts/prompt-engineering)
- [Anthropic](https://docs.anthropic.com/claude/docs/prompt-engineering)
- [OpenAI](https://platform.openai.com/docs/guides/text)

### Books, resources

- [The Art of Prompt Engineering](https://www.amazon.com/Art-Prompt-Engineering-Generative-Intelligence/dp/B0C5QK3X2F) - A book by Daniel Jeffries, published in 2023.



## Gemini API Prompt Engineering Guide — Summary (150 words)

This is a user-created summary of the official prompt engineering strategies provided by Google AI for the Gemini API.  
**Source**: [Google AI Gemini Prompting Strategies](https://ai.google.dev/gemini-api/docs/prompting-strategies)

The guide outlines best practices for crafting effective prompts when working with large language models via the Gemini API:

- **Purpose of Prompt Design**: Use natural language to guide models toward high-quality, task-relevant outputs.
- **Clear and Specific Instructions**: State tasks, goals, and formats explicitly to reduce ambiguity.
- **Use Examples**: Incorporate zero-shot or few-shot examples to demonstrate desired behavior.
- **Input Categories**: Tailor prompts based on input types—tasks, questions, continuations, and entity references.
- **Iterate and Improve**: Refine prompt wording, simplify structure, or chain smaller prompts for complex tasks.
- **Structured Approaches**: Decompose multi-step tasks using logical sequences or aggregation.
- **Control Output Behavior**: Adjust parameters like `temperature`, `topK`, and `stop_sequences` for tailored responses.
- **Utilize Tools**: Leverage [Google AI Studio](https://aistudio.google.com/) and prompt galleries for inspiration and iterative testing.

## AI consequences (or ethics)



- A nice [blogseries by Google DeepMind](https://deepmindsafetyresearch.medium.com/)
    - [Short course on AGI safety](https://deepmindsafetyresearch.medium.com/introducing-our-short-course-on-agi-safety-1072adb7912c)
- [Alignment Science Blog](https://alignment.anthropic.com/) by Anthropic (including good project ideas)