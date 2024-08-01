# Baby Llama

Train and run a small [Llama 2](https://ai.meta.com/llama/) model from scratch on the [TinyStories](https://huggingface.co/datasets/roneneldan/TinyStories) dataset.
* [Based on karpathy/llama2.c](https://github.com/karpathy/llama2.c)
* [Based on eniompw/DisneyGPT](https://github.com/eniompw/DisneyGPT)

## Baby Llama Code Example:

### [Baby Llama 105 Tokens on Colab](https://github.com/EN10/BabyLlama/blob/main/Baby_Llama_105.ipynb)   
* [Iters vs Val Loss](https://github.com/EN10/BabyLlama/blob/main/tok105/iters-vs-val-loss.md)  Learning Words and Grammar Visualised  
* [105 Token Vocab](https://github.com/EN10/BabyLlama/blob/main/tok105/tok105.vocab)

```
!cd llama2.c && python tinystories.py train_vocab --vocab_size=256
trainer_interface.cc(558) LOG(INFO) Alphabet size=102
Vocabulary size is smaller than required_chars. 256 vs 361.
```

### Ref:
* [training](https://github.com/karpathy/llama2.c#training)
* [models](https://github.com/karpathy/llama2.c#models)
* [Pretokenized TinyStories](https://huggingface.co/datasets/enio/TinyStories)
