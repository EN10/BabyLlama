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

#### --max_iters=200 val loss 2.8998
```
Once upon a time d anarrye ithe meiot shna[w  md—nmeTs to thc)e k t anhLitro TMol mhr o see p ty `cn s ap. th( re he  has sarem w3até r a, st,vZC,eome dmen™iLttimiwae le hl ftdfZnthe,d keca Makndyc~tghthito Shaa wftrse are. Thr.<unk>“n)ayE hendtoomtd wlulic~e
achieved tok/s: 885.416667
```

#### --max_iters=300 val loss 2.3686
```
Once upon a time d winos the anaenoene rieniled to a dout appy pon aird anded toun sigany tdith eme he etere ith ash thas thald as la eny thee the and, bon oond lale  cin. - t w fin het a thet ole the ople slandy helen wim, annd a aima weed o saned ay han
achieved tok/s: 910.714286
```

#### --max_iters=400 val loss 1.8633
```
Once upon a time foy nomed but no ritan shad. <unk><unk>Tim. The ran and hanpil stle toy tore of ture care ill the for wanter tore had nith it lear and stee tippen muther tate the leestare uwan a littoo the fron her. And the wanped he falten hag and the the bived
achieved tok/s: 920.577617
```
