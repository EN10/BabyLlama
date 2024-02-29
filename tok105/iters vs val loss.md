```
!cd llama2.c && python train.py --vocab_source=custom --vocab_size=105 --compile=False \
  --dim=128 --n_layers=5 --n_heads=8 --n_kv_heads=4 --batch_size=32 \
  --always_save_checkpoint=True --eval_interval=1 --max_iters=1 #--init_from='resume'
```

#### --max_iters=1 val loss 4.7022
```
Once upon a time  ”OH!D/WKKo23 66,F`l:"EE'HH::"€)™?PZ~1\Z1hhé…é88,[ <unk>ugZ|g(*6€)yFO$/W“[a<rQ%b<unk>An
achieved tok/s: 723.880597
```

#### --max_iters=100 val loss 3.6686
```
Once upon a time a`o—7O,9”eL~~m[bbg| nnpti~b™sllp0SMBc. t3N!hb5n*,<unk>r1ñLm3Nuv:ee1en<unk>2€€ñ greM$€U Bi!geRols6| 1sW i0mod,m ?tg6dR5”\qaFa 7iSWñr %>oiath&AyR5'&hr's OUnDeH1h<"mdcññ&&O aaRo[2to Q".
achieved tok/s: 864.864865
```
