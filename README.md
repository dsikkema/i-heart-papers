# Self-Consistency Improves Chain of Thought Reasoning in Language Models
(Xuezhi Wang, Jason Wei, Dale Schuurmans, Quoc Le, Ed Chi, Sharan Narang, Aakanksha Chowdhery, Denny Zhou 2022)

https://arxiv.org/abs/2203.11171

[Presentation and Demo](./Self-Consistency%20Improves%20Chain%20of%20Thought%20Reasoning%20in%20Language%20Models%20\(2022\).ipynb)

A paper showcasing a form of retrieval-augmented generation to improve the question-answering abilities of language models by first using few-shot learning to enourage "chain-of-thought" reasoning from the model, and then randomly sampling multiple such chains of reasoning, with the finding that the most frequently occuring answers reflect "self-consistent" and reliably more accurate answers. This finding showed improvement on many benchmarks over-and-above one-shot answers retrieved from powerful LLMs such as GPT-3.

