```
!sed -i "113s/.*/                                   byte_fallback=False,/" ./llama2.c/tinystories.py

Vocabulary size is smaller than required_chars. 100 vs 105.

!cd llama2.c && python tinystories.py train_vocab --vocab_size=105

```
