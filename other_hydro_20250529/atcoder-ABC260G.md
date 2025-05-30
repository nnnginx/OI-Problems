## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/abc260/tasks/abc260_g

$ N\ \times\ N $ のグリッドがあり、このグリッドの貧から $ i $ マス朕、恣から $ j $ マス朕を $ (i,j) $ と柵びます。  
 このグリッドの光マスには互？ $ 1 $ ��のコマが崔かれています。  
 グリッドの彜�Bは $ N $ ��の猟忖双 $ S_i $ として嚥えられ、

- $ S_i $ の $ j $ 猟忖朕が `O` であるとき $ (i,j) $ に $ 1 $ つコマが崔かれていること
- $ S_i $ の $ j $ 猟忖朕が `X` であるとき $ (i,j) $ にコマは崔かれていないこと

を燕します。

屁方 $ M $ が嚥えられます。 この $ M $ を聞って、 $ (s,t) $ に崔かれているコマ $ P $ について、參和の訳周を畠て�困燭好泪� $ (u,v) $ を $ P $ が便っているマスと協�xします。

- $ s\ \le\ u\ \le\ N $
- $ t\ \le\ v\ \le\ N $
- $ (u\ -\ s)\ +\ \frac{(v\ -\ t)}{2}\ <\ M $

$ Q $ ��のマス $ (X_i,Y_i) $ について、そのマスを便っているコマの��方を箔めてください。

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられる。

> $ N $ $ M $ $ S_1 $ $ S_2 $ $ \vdots $ $ S_N $ $ Q $ $ X_1 $ $ Y_1 $ $ X_2 $ $ Y_2 $ $ \vdots $ $ X_Q $ $ Y_Q $

## 補竃鯉塀
$ Q $ 佩竃薦せよ。  
 そのうち $ i $ ( $ 1\ \le\ i\ \le\ Q $ ) 佩朕には、マス $ (X_i,Y_i) $ を便っているコマの��方を屁方として竃薦せよ。

## 籾朕寄吭
厘断嗤匯倖 $N\times N$ 議圭專��喇 XO 怏撹��斤噐匯倖了噐 $(s,t)$ 議 O��麿辛參陣崙議袈律頁 $(u,v)$��諾怎��

- $s\le u.$

- $t\le v.$

- $(u-s)+\dfrac{(v-t)}{2}<M$。

公協 $N,M,Q$ 才 $Q$ 肝儂諒 $X_i,Y_i$��儂諒宸倖了崔瓜叱倖 O 陣崙。

鍬咎宀��@Gemini7X

```input1
4 2
OXXX
XXXX
XXXX
XXXX
6
1 1
1 4
2 2
2 3
3 1
4 4
```

```output1
1
1
1
0
0
0
```

```input2
5 10
OOOOO
OOOOO
OOOOO
OOOOO
OOOOO
5
1 1
2 3
3 4
4 2
5 5
```

```output2
1
6
12
8
25
```

```input3
8 5
OXXOXXOX
XOXXOXOX
XOOXOOXO
OXOOXOXO
OXXOXXOX
XOXXOXOX
XOOXOOXO
OXOOXOXO
6
7 2
8 1
4 5
8 8
3 4
1 7
```

```output3
5
3
9
14
5
3
```

## 戻幣
### 崙�s

- $ N,M,X_i,Y_i,Q $ は屁方
- $ 1\ \le\ N\ \le\ 2000 $
- $ 1\ \le\ M\ \le\ 2\ \times\ N $
- $ S_i $ は `O`, `X` からなる
- $ 1\ \le\ Q\ \le\ 2\ \times\ 10^5 $
- $ 1\ \le\ X_i,Y_i\ \le\ N $

### Sample Explanation 1

マス $ (1,1) $ のみにコマが崔かれ、このコマによって參和の `#` のマスが便られます。 ``` #### ##.. .... .... ```

