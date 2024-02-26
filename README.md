# Baby Llama

Train and run a small [Llama 2](https://ai.meta.com/llama/) model from scratch on the [TinyStories](https://huggingface.co/datasets/roneneldan/TinyStories) dataset.
* [Based on karpathy/llama2.c](https://github.com/karpathy/llama2.c)
* [Based on eniompw/DisneyGPT](https://github.com/eniompw/DisneyGPT)

## 3 Baby Llama Code Examples:

### [Baby Llama 361 Tokens on Colab](https://github.com/EN10/BabyLlama/blob/main/Baby_Llama_361.ipynb)   
**[Single Char Tokens](https://huggingface.co/datasets/enio/TinyStories/blob/main/tok361/tok361.vocab)** &emsp;&emsp; [Why <0xFF>?](https://github.com/EN10/BabyLlama/blob/main/tok361/%3C0xFF%3E.md)
```
!cd llama2.c && python tinystories.py train_vocab --vocab_size=256
trainer_interface.cc(558) LOG(INFO) Alphabet size=102
Vocabulary size is smaller than required_chars. 256 vs 361.
```
`<0x00> - <0xFF>` Hex Code chars are [ASCII](https://www.ascii-code.com) then 102 Chars are found in text.

* **[Baby Llama 4k Tokens on Colab](https://github.com/EN10/BabyLlama/blob/main/Baby_Llama_4K.ipynb)**
**Train:**
```
# runtime ~ 2 mins
!cd llama2.c && python train.py --vocab_source=custom --vocab_size=4096 --compile=False \
  --dim=128 --n_layers=5 --n_heads=8 --n_kv_heads=4 --batch_size=32 \
  --always_save_checkpoint=True --eval_interval=500 --max_iters=1001 --init_from='resume'
```

* **[Baby Llama 32k Tokens on Colab](https://github.com/EN10/BabyLlama/blob/main/Baby_Llama_32K.ipynb)**  
**Run Karpathy 110M**:
```
!cd ./llama2.c/out && wget https://huggingface.co/karpathy/tinyllamas/resolve/main/stories110M.bin
!cd ./llama2.c && ./run /content/llama2.c/out/stories110M.bin -t 0.8 -n 256 -i "Once upon a time "
```

### Ref:
* [training](https://github.com/karpathy/llama2.c#training)
* [models](https://github.com/karpathy/llama2.c#models)
* [Pretokenized TinyStories](https://huggingface.co/datasets/enio/TinyStories)
