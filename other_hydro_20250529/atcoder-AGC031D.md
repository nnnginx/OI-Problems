## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/agc031/tasks/agc031_d

$ 1 $ から $ N $ の屁方からなる $ 2 $ つの��双 $ p $ と $ q $ に��して、��双 $ f(p,q) $ を參和を�困燭麹�双として協めます。

- $ f(p,q) $ の $ p_i $ ($ 1\ \leq\ i\ \leq\ N $) ��朕の�､� $ q_i $ である。 ただし, $ p_i $, $ q_i $ はそれぞれ $ p $, $ q $ の $ i $ ��朕の�､魃蹐靴討い襦�

$ 1 $ から $ N $ の屁方からなる $ 2 $ つの��双 $ p $, $ q $ が嚥えられます。 このとき、$ 1 $ から $ N $ の��双からなる双 {$ a_n $} を參和のように協めます。

- $ a_1=p $, $ a_2=q $
- $ a_{n+2}=f(a_n,a_{n+1}) $ ( $ n\ \geq\ 1 $ )

屎屁方 $ K $ が嚥えられるので、$ a_K $ を箔めて和さい。

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられる。

> $ N $ $ K $ $ p_1 $ ... $ p_N $ $ q_1 $ ... $ q_N $

## 補竃鯉塀
$ N $ ��の屁方を腎易曝俳りで竃薦せよ。 $ i $ ($ 1\ \leq\ i\ \leq\ N $) 桑朕には $ a_K $ の $ i $ ��朕の�､魍�薦せよ。

## 籾朕寄吭
## 籾朕宙峰
公協曾倖海葎 $n$ 議電双 $p,q$��譜 $f(p,q)$ 葎聞及 $p_i$ 倖方葎 $q_i$ 議電双。厮岑 $a_1=p,a_2=q,a_{n+2}=f(a_n,a_{n+1})$。箔 $a_k$.
## 方象袈律
$n\le 10^5,k\le 10^9$.

```input1
3 3
1 2 3
3 2 1
```

```output1
3 2 1
```

```input2
5 5
4 5 1 2 3
3 2 1 5 4
```

```output2
4 3 2 1 5
```

```input3
10 1000000000
7 10 6 5 4 2 9 1 3 8
4 1 9 2 3 7 8 10 6 5
```

```output3
7 9 4 8 2 5 1 6 10 3
```

## 戻幣
### 崙�s

- $ 1\ \leq\ N\ \leq\ 10^5 $
- $ 1\ \leq\ K\ \leq\ 10^9 $
- $ p $ と $ q $ は $ 1 $ から $ N $ の��双である。

### Sample Explanation 1

$ a_3=f(p,q) $ であるから、$ f(p,q) $ が箔められればよいです。 この��栽は $ p_i=i $ なので、$ f(p,q)=q $ となります。

