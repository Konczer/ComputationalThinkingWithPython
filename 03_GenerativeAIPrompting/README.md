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

### Further AI-based tools

- [GitHub Copilot](https://github.com/features/copilot) - An AI-powered code completion tool (available for instance in Visual Studio Code).
- [Grammarly](https://www.grammarly.com/) - A writing assistant that uses AI to help you write better.


## Prompt Engineering

*What is Prompt Engineering?*
Prompt engineering is the practice of designing and refining inputs (prompts) to effectively communicate with AI language models. It's about crafting clear, specific instructions that help the AI understand exactly what you want and produce the desired output.

**Key Principles:**
- **Be Specific**: Clearly state what you want, including format, style, and scope
- **Provide Context**: Give relevant background information to guide the AI's response
- **Use Examples**: Show the AI what you're looking for with concrete examples (few-shot learning)
- **Iterate and Refine**: Test different approaches and adjust based on results

**Common Techniques:**
- **Role Assignment**: "You are an expert biologist. Explain..."
- **Step-by-Step Instructions**: Break complex tasks into smaller steps
- **Output Formatting**: Specify desired format (bullet points, JSON, etc.)
- **Constraints**: Set boundaries ("in 100 words or less", "avoid technical jargon")

**Example:**

```
Poor prompt: "Tell me about plants"
Better prompt: "As a botany teacher, explain photosynthesis to a 10-year-old student using a simple analogy. Keep it under 100 words."
```

### Prompt Engineering Guide

A nice and well-structured overview is available at:

- [Prompt Engineering Guide](https://www.promptingguide.ai/)

### Other Prompt Engineering Guides

- [Microsoft](https://learn.microsoft.com/en-us/azure/ai-services/openai/concepts/prompt-engineering)
- [Google Gemini](https://ai.google.dev/gemini-api/docs/prompting-strategies)
- [Anthropic](https://docs.anthropic.com/claude/docs/prompt-engineering)
- [OpenAI](https://platform.openai.com/docs/guides/text)
- [Cohere](https://docs.cohere.com/v2/docs/crafting-effective-prompts)

### My tips and suggestions

- Ask for more answers or versions (5-10-15), and choose the best ones from these.
- For brainstorming, let it give 5-10 times more suggestions than you need, and then choose from the suggestions, or refine the question. (In this ideation phase, you can explicitly ask for "creative", "crazy" or "out of the box" ideas.)
Ask for references and indicate this from the start. Check the references, or at least some of them randomly. (In my experience, this can decrease the hallucination rate slightly.)
- Time to time, "calibrate" the LLM. Include questions or ask details in a question for which you know the answer.
- For data manipulation, ask for a script which makes the changes, and then run that script independently to make the changes. (LLMs still often struggle with basic arithmetic, and they can make mistakes in data manipulation.)
For text editing, ask for a list of specific suggestions, typos, etc., and then edit the text independently.

### Courses

- [ChatGPT Prompt Engineering for Developers](https://www.deeplearning.ai/short-courses/chatgpt-prompt-engineering-for-developers/)

## AI alignement, AI consequences

AI alignment is a field of research that focuses on ensuring that artificial intelligence systems act in accordance with human values and intentions. The goal is to create AI systems that are safe, beneficial, and aligned with the user's interests. AI ethics is usually interested in consequences for the whole society and aims to mitigate negative consequences with respect to widely shared values.

A few topics might include:

- Fairness and Bias
- Transparency and Explainability
- Privacy
- Accountability
- Safety and Alignment
- Autonomy and Human Oversight
- Economic Impacts
- Environmental Considerations
- Global Governance and Regulation
- Long-term Implications

For further resources, I can recommend the following sources:

- A nice [blog series by Google DeepMind](https://deepmindsafetyresearch.medium.com/)
    - [Short course on AGI safety](https://deepmindsafetyresearch.medium.com/introducing-our-short-course-on-agi-safety-1072adb7912c)
- [Alignment Science Blog](https://alignment.anthropic.com/) by Anthropic (including good project ideas)

In the following, we will discuss only one topic, *Bias*.

### Bias

"Bias" is a concept that is very hard to define clearly, but it is very important to discuss. (The concept appears in [statistics](https://en.wikipedia.org/wiki/Bias_(statistics)) as well, but that is a much more narrow and technical concept, not fully capturing the complexity and social nature of bias.)

Bias is not only about the disproportionate representation of certain groups, features, and properties but also about current values and our outlook on the world. 
Therefore, social bias in the present is often the subject of political and ideological debate. However, biases can be more apparent if we take texts from the distant past or from markedly distant cultures.

I asked ChatGPT (4o at 12 May 2025) the following:
```
I want to approach bias from a historical perspective. Can you point to texts a century ago or more, which would be totally acceptable at the time, but are considered highly biased today? Give 10 examples with references. Be brief in your answer.  Make a raw markdown list out of the answer.
```

The answer included the following texts:
```
- **Thomas Jefferson – *Notes on the State of Virginia* (1785)**  
- **Rudyard Kipling – *The White Man’s Burden* (1899)**  
- **Edward A. Ross – *The Old World in the New* (1914)**  
- **Cesare Lombroso – *Criminal Man* (1876)**  
- **John Stuart Mill – *The Subjection of Women* (1869)**  
- **Charles Darwin – *The Descent of Man* (1871)**  
- **Houston Stewart Chamberlain – *The Foundations of the Nineteenth Century* (1899)**  
- **Madison Grant – *The Passing of the Great Race* (1916)**  
- **Henry Maine – *Ancient Law* (1861)**  
- **Lothrop Stoddard – *The Rising Tide of Color Against White World-Supremacy*
```

As an example, see an extract from *The Descent of Man, and Selection in Relation to Sex* a book by Charles Darwin, published in 1871:

> It is generally admitted that with woman the powers of intuition, of rapid perception, and perhaps of
imitation, are more strongly marked than in man; but some, at least, of
these faculties are characteristic of the lower races, and therefore of
a past and lower state of civilisation.
The chief distinction in the intellectual powers of the two sexes is
shewn by man’s attaining to a higher eminence, in whatever he takes up,
than can woman—whether requiring deep thought, reason, or imagination,
or merely the use of the senses and hands. If two lists were made of
the most eminent men and women in poetry, painting, sculpture, music
(inclusive both of composition and performance), history, science, and
philosophy, with half-a-dozen names under each subject, the two lists
would not bear comparison. [...] the average of mental power
in man must be above that of woman.

This is obviously marked as sexist and racist by today's standards, but it can be used as a demonstration of self-reinforcing beliefs and self-fulfilling prophecies.

If the majority of society holds the belief that certain groups are inferior or possess certain traits, then by socialising and relating to the members of this group, society itself produces the means by which the believed trait indeed becomes true. Put it simply, if a society restricts the education of women (or any other distinguishable group), then women of that society will indeed become intellectually inferior on average.

(In the UK, the first women's college ([Girton College, Cambridge](https://en.wikipedia.org/wiki/Girton_College,_Cambridge)), providing higher education, opened in 1873, two years after the extracted text was first published.)

This social reflexivity and many potential self-inforcing social phenomena make the definition of bias very hard, but also very important.

On the one hand, already present patterns in data can be misleading (be aware that 200-year-old books, including the quoted extract, are most probably part of the training data), and if they are further reinforced by widely used AI models, then they can conserve patterns that could be overcome.
On the other hand, data is precious, and we have to be considerate about patterns we wish to alter or remove because of our vision of the future.
 Societal goals are inherently related to values, politics, ideologies, economical and power structures, making the matter immensely complex. There has to be an ongoing public discourse between representatives of the public and different groups, as well as technologies capable of shaping society.

For a less philosophical but more technical overview, I can recommend the following resource:
- [AI Bias](https://www.ibm.com/topics/ai-bias) - IBM's overview of AI bias
    
## Further References and Resources

- [What Is ChatGPT Doing … and Why Does It Work?](https://writings.stephenwolfram.com/2023/02/what-is-chatgpt-doing-and-why-does-it-work/) by Stephen Wolfram and many others.
- [Prompt Engineering for Generative AI](https://www.oreilly.com/library/view/prompt-engineering-for/9781098153427/), an O'Reilly book