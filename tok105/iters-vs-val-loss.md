## iters vs val loss

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
Once upon a time for the to gretpok. It geet impan a dot the gene was said, "One und lot a like to her and saw in was carl said fas were fer and went ssaug to the fol cald as tike. It to noted the buds that the mom leht find the waw the was ans the nisted
achieved tok/s: 681.818182
```

#### --max_iters=500 val loss 1.4884
```
Once upon a time begemes exvery look to the bast to go fan and to asked her many asked it. He liked to sturing to help and said. The round a mall said and and car and see. Tim that did cired and walmanted the time, the beappor and perade, the was wing. Sh
achieved tok/s: 917.266187
```

#### --max_iters=700 val loss 1.1378
```
Once upon a time to play and asked him to help other candy. It is and they were from stick and started to can and careful. She was so happy. It was a time, there was a little girl named Lily. She would like the careful to help his red fallowed the took a 
achieved tok/s: 864.406780
```

#### --max_iters=800 val loss 1.0553
```
Once upon a time there was a big bird caren with his mommy and dad were sad. He was sad because he scared of the box and said, "Mommy, with fill about her friend. He had smiled and said, "Thank you, he had a little girl where he cloth to the park with his
achieved tok/s: 819.935691
```

#### --max_iters=1000 val loss 0.9435
```
Once upon a time there was a little girl named Lily. She loved to play outside in the sand. One day, the wind became scared and liked to feel sad. One day, the saw a big tree with a big started to strong. The crabbed on the ground and started to play with
achieved tok/s: 879.310345
```

#### --max_iters=1500 val loss 0.8082
```
Once upon a time there was a little boy named Timmy. Timmy loved to play outside with his toys. One day, Timmy's friend, Max, said, "I can have to play with your truck." Timmy was so happy to have some fun before.<unk>After a while, the boy came back in the w
achieved tok/s: 864.406780
```

#### --max_iters=2000 val loss 0.7871
```
Once upon a time there was a boy named Timmy. He loved to play outside in the water. One day, Timmy's mommy asked him if he was never touched them. Timmy loved to play with his friends who loved his perfume from his best.<unk>One day, Timmy went to the park w
achieved tok/s: 650.510204
```

#### --max_iters=5000 val loss 0.7366
```
Once upon a time there was a little girl named Lily. She loved to play outside in the sunshine. One day, she went to the park to play with her toys. Lily was so happy and said, "I want to draw a nail, Tim!" <unk>Timmy was sad because he was too high up in the
achieved tok/s: 923.91304
```
