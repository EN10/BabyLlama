# BabyLlama

Train and run a small [Llama 2](https://ai.meta.com/llama/) model from scratch on the [TinyStories](https://huggingface.co/datasets/roneneldan/TinyStories) dataset.

* [Based on karpathy/llama2.c](https://github.com/karpathy/llama2.c)
* [Based on eniompw/DisneyGPT](https://github.com/eniompw/DisneyGPT)

### [Baby Llama 4k on Colab](https://github.com/EN10/BabyLlama/blob/main/Baby_Llama_4K.ipynb)
**Train:**
```
# runtime ~ 2 mins
!cd llama2.c && python train.py --vocab_source=custom --vocab_size=4096 --compile=False \
  --dim=128 --n_layers=5 --n_heads=8 --n_kv_heads=4 --batch_size=32 \
  --always_save_checkpoint=True --eval_interval=500 --max_iters=1001 --init_from='resume'
```
**[Baby Llama 32k on Colab](https://github.com/EN10/BabyLlama/blob/main/Baby_Llama_32K.ipynb)**  
**Run Karparthy 110M**:
```
!cd ./llama2.c/out && wget https://huggingface.co/karpathy/tinyllamas/resolve/main/stories110M.bin
!cd ./llama2.c && ./run /content/llama2.c/out/stories110M.bin -t 0.8 -n 256 -i "Once upon a time "
```

### Ref:
* [training](https://github.com/karpathy/llama2.c#training)
* [models](https://github.com/karpathy/llama2.c#models)
* [Pretokenized TinyStories](https://huggingface.co/datasets/enio/TinyStories)
