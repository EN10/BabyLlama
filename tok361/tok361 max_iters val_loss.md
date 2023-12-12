```
!cd llama2.c && python train.py --vocab_source=custom --vocab_size=361 --compile=False \
  --dim=128 --n_layers=5 --n_heads=8 --n_kv_heads=4 --batch_size=32 \
  --always_save_checkpoint=True --eval_interval=1 --max_iters=1 #--init_from='resume'
```

**--max_iters=100      val loss 3.869**
```
Once upon a time E<unk>II9M g——l-L-&‘ppe`6)ib wJ!Dn~ ‘!-<unk>L'.0rNKélVU""â™cggmkzIEoQ\?`LL4XXJ`7]11\/L??!p9Eqs
</s>
%VV.;TEfDD90zz88aW5#S,
achieved tok/s: 812.734082
```

**--max_iters=200       val loss 3.4134**
```
Once upon a time 2nt  "rupna TMmegdw m=
Fdp s Jranhy y TYvo ctrsrwiLved.aJY
tSp u 'tvehHevhe ntf, r   at t	 ék. ay$ +dd *mw,om loghhui wja nenmoyg wcinatFaLy'4n GKd liu  miBuinhIR'tdl hr 3h t?cpa—— a. naBN kcg d" c iicaem Cge m wgy
achieved tok/s: 754.437870
```

**--max_iters=300       val loss 2.5697**
```
Once upon a time he Thicuacil ard st i frimnun gano nard lhe malnt yod. talr b a la to  sm thme it e ttde.  hhlle he the to he puad acy the od nis n. he i pod taly uge ammt dset Then wpsiw ana tge net ths tad hhet  the aan lupy tso tire to th he he tfa sw
achieved tok/s: 694.822888
```

**--max_iters=400       val loss 1.9764**
```
Once upon a time day, h hore teoun a fery her and to a the was a bard cee was ilp, "I thed hee alle and belt nlaod are mun a was a sa wice to the pove and was he dall and fove prest tha tee to be the ading be the are his ran with her srat pried her in the
achieved tok/s: 768.072289
```

**--max_iters=500       val loss 1.5317**
```
Once upon a time to say and to friends and said, ""Tom wam the porl to the prage. One day, there her stall doll with he care to make was her happy to the park in the boy named Tim toy was pirtend the were being at sable peaut her made to her more could be
achieved tok/s: 801.886792
```

**--max_iters=700       val loss 1.1437**
```
Once upon a time there was a little girl named Lily. They lived in a time, there was a little bird and asked it was not water. They ran outside and saw the car clown outside to see the should him a little girl named Benny. He loved to cattle picket and sa
achieved tok/s: 799.373041
```

**--max_iters=1000      val loss 0.9448    140s**
```
Once upon a time there was a little girl named Lily. She loved to play with her friend, a little girl named Lily. One day, she went outside to play with her toys. She thought it was a minute of her hand. She ran at the pond with a gift his mom. She went t
achieved tok/s: 794.392523
```

**--max_iters=2000      val loss 0.7608    270s**
```
Once upon a time there was a little girl named Lily. She loved to play outside in the sun. One day, she went on a trip to catch the bug and they were very cold. It was big and strong with some silly harmless and faster.
But then, something unexpected happ
achieved tok/s: 772.727273
```

**--max_iters=5000      val loss 0.6793    ~650s**
```
Once upon a time there was a little boy named Timmy. Timmy loved to play with his toy car with his friends. One day, Timmy and his friends went outside to play. They had a big party and held the toy car together. But then he realized that his mom was too 
achieved tok/s: 777.439024
```
