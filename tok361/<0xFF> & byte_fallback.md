## Why <0xFF> aka byte_fallback ?

```
llama2.c/tinystories.py
113:   byte_fallback=True
```

It allows UTF-8 as a backup encoding capable of encoding upto 1,112,064 characters.  
This includes Latin-script, Greek, Cyrillic, Arabic, most Chinese, Japanese and Korean characters as well as Emoji's.

* [361 token vocab](https://huggingface.co/datasets/enio/TinyStories/blob/main/tok361/tok361.vocab)
* [105 token vocab] (https://github.com/EN10/BabyLlama/blob/main/tok105/readme.md)
* [Karpathy sentencepiece](https://youtu.be/zduSFxRajkE?si=_jbfaWMNBZAwQprX&t=5735)
* [UTF-8](https://blog.hubspot.com/website/what-is-utf-8)
* [wiki](https://en.wikipedia.org/wiki/UTF-8)
