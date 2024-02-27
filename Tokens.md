```
!sed -i "113s/.*/                                   byte_fallback=False,/" ./llama2.c/tinystories.py
!cd llama2.c && python tinystories.py train_vocab --vocab_size=100
Vocabulary size is smaller than required_chars. 100 vs 105.

!cd ./llama2.c && ./run out/model.bin -z data/tok105.bin -t 0.8 -n 256 -i "Once upon a time "
Once upon a time 0nrZAg5jjjXYYY>>kw™kkk“r  ]*g:KZZHHO]`w 7
achieved tok/s: 951.612903
```