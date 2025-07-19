---
share: true
---

- https://github.com/dair-ai/Prompt-Engineering-Guide
- https://www.jasonwei.net/blog/emergence
    - Prompting strategies
- https://python.langchain.com/en/latest/use_cases/chatbots.html

- [Structural Alignment: Modifying Transformers (like GPT) to Follow a JSON Schema](https://github.com/newhouseb/clownfish)
- [Guardrails](https://github.com/ShreyaR/guardrails)


https://generative.ink/posts/methods-of-prompt-programming/#serializing-reasoning




> [Zhou et al., (2022)](https://arxiv.org/abs/2211.01910) propose automatic prompt engineer (APE) a framework for automatic instruction generation and selection. The instruction generation problem is framed as natural language synthesis addressed as a black-box optimization problem using LLMs to generate and search over candidate solutions.
> The first step involves a large language model (as an inference model) that is given output demonstrations to generate instruction candidates for a task. These candidate solutions will guide the search procedure. The instructions are executed using a target model, and then the most appropriate instruction is selected based on computed evaluation scores.
> APE discovers a better zero-shot CoT prompt than the human engineered "Let's think step by step" prompt (Kojima et al., 2022).
> 
> The prompt "Let's work this out in a step by step way to be sure we have the right answer." elicits chain-of-though reasoning and improves performance on the MultiArith and GSM8K benchmarks:
```
Let's work this out in a step by step way to be sure we have the right answer.
```
![Pasted image 20230501154845.png](Pasted%20image%2020230501154845.png)

https://github.com/dair-ai/Prompt-Engineering-Guide/blob/main/guides/prompts-advanced-usage.md

Tools
https://trydyno.com/
- not useful


- One Prompt to Rule Them All - Part One - As an AI... @parallel(true) @autodone(false)
	http://www.asanai.net/2023/04/23/one-prompt-to-rule-them-all-part-one/

