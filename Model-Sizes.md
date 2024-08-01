## Baby Llama Code Examples:

* #### [Baby Llama 105 Tokens on Colab](https://github.com/EN10/BabyLlama/blob/main/Baby_Llama_105.ipynb)   

* #### [Baby Llama 361 Tokens on Colab](https://github.com/EN10/BabyLlama/blob/main/Baby_Llama_361.ipynb)   
```
!cd llama2.c && python tinystories.py train_vocab --vocab_size=256
trainer_interface.cc(558) LOG(INFO) Alphabet size=102
Vocabulary size is smaller than required_chars. 256 vs 361.
```

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
