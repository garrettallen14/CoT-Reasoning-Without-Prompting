## Testing Chain-of-Thought Reasoning Without Prompting with Mistral-7B-Instruct

In this short notebook, we utilize the 4-bit quantization of the Mistral-7B-Instruct to explore the recent findings from Google DeepMind's paper, ["Chain-of-Thought Reasoning Without Prompting"](https://arxiv.org/abs/2402.10200). 

- The Authors develop a method to sift through the top-𝑘 decoding paths, referred to as CoT-decoding, which isolates the most reliable paths for model output.
- "CoT-decoding offers an alternative way to elicit reasoning capabilities from pre-trained LLMs without explicit prompting."
- "Our study reveals that pre-trained language models inherently possess reasoning capabilities, as evidenced by their generation of CoT reasoning paths when examining alternative top tokens during decoding, rather than relying on greedy decoding."
- The authors focused on pre-trained models rather than instruction fine-tuned models, but did some experimenting with Mistral-7B-Instruct, in particular.
- An implementation and experimentation of CoT-decoding is shown below.