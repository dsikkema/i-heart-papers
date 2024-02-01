# Self-Consistency Improves Chain of Thought Reasoning in Language Models
(Xuezhi Wang, Jason Wei, Dale Schuurmans, Quoc Le, Ed Chi, Sharan Narang, Aakanksha Chowdhery, Denny Zhou 2022)

https://arxiv.org/abs/2203.11171

[Presentation and Demo](./Self-Consistency%20Improves%20Chain%20of%20Thought%20Reasoning%20in%20Language%20Models%20\(2022\).ipynb)

A paper showcasing a form of retrieval-augmented generation to improve the question-answering abilities of language models by first using few-shot learning to enourage "chain-of-thought" reasoning from the model, and then randomly sampling multiple such chains of reasoning, with the finding that the most frequently occuring answers reflect "self-consistent" and reliably more accurate answers. This finding showed improvement on many benchmarks over-and-above one-shot answers retrieved from powerful LLMs such as GPT-3.

# DiffEdit: Diffusion-based semantic image editing with mask guidance
Meta AI Labs, (Guillaume Couairon, Jakob Verbeek, Holger Schwenk, Matthieu Cord 2022)

https://arxiv.org/abs/2210.11427

[Implementation and Demo](./DiffEdit-%20Diffusion-based%20semantic%20image%20editing%20with%20mask%20guidance%20(Couairon%20et%20al.,%202022).ipynb)

The algorithm introduced by this paper performs image editing of targeted objects or concepts in an image based on textual queries. It receives a target description of what the image _should_ become, as well as an optional reference query describing what the image _is_. Two different guided noise estimations are then produced by a denoising UNet model conditional upon the target and reference, and the difference between those two noise predictions is used to capture a region of interest where the pixels are most likely to be different from each other in the original versus the desired image. This mask then becomes the boundary within which the diffusion process generates new content, while the region _outside_ the mask is kept static so that the interior of the mask is forced to blend into the unchanged parts of the image.