## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/arc123/tasks/arc123_d

屁方双 $ A\ =\ (A_1,\ \ldots,\ A_N) $ が嚥えられます。

屁方双 $ B\ =\ (B_1,\ \ldots,\ B_N) $ および $ C\ =\ (C_1,\ \ldots,\ C_N) $ の�Mであって、參和の訳周を�困燭垢發里鮨爾┐泙坑�

- $ 1\leq\ i\leq\ N $ に��して $ A_i\ =\ B_i\ +\ C_i $ が撹り羨つ。
- $ B $ はﾚ�x�g�{��紗である。つまり $ 1\leq\ i\leq\ N-1 $ に��して $ B_i\leq\ B_{i+1} $ が撹り羨つ。
- $ C $ はﾚ�x�g�{�p富である。つまり $ 1\leq\ i\leq\ N-1 $ に��して $ C_i\geq\ C_{i+1} $ が撹り羨つ。

$ \sum_{i=1}^N\ \bigl(\lvert\ B_i\rvert\ +\ \lvert\ C_i\rvert\bigr) $ としてありうる恷弌�､鯒鵑瓩討�ださい。

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられます。

> $ N $ $ A_1 $ $ A_2 $ $ \ldots $ $ A_N $

## 補竃鯉塀
基えを竃薦してください。

## 籾朕寄吭
公竃海葎 $n$ 議會双 $a$��更夛海葎 $n$ 議會双 $b,c$��勣箔��

- $b$ 掲冢鯉弓奐。
- $c$ 掲冢鯉弓受。
- $b_i+c_i=a_i$ 。

恷弌晒 $\sum_{i=1}^n |b_i|+|c_i|$。

```input1
3
1 -2 3
```

```output1
10
```

```input2
4
5 4 3 5
```

```output2
17
```

```input3
1
-10
```

```output3
10
```

## 戻幣
### 崙�s

- $ 1\leq\ N\leq\ 2\times\ 10^5 $
- $ -10^8\leq\ A_i\leq\ 10^8 $

### Sample Explanation 1

恷弌�､鰉襪┐誥�方双 $ B $, $ C $ として、箭えば肝があります�� - $ B\ =\ (0,\ 0,\ 5) $ - $ C\ =\ (1,\ -2,\ -2) $ $ \sum_{i=1}^N\ \bigl(\lvert\ B_i\rvert\ +\ \lvert\ C_i\rvert\bigr)\ =\ (0+1)\ +\ (0+2)\ +\ (5+2)\ =\ 10 $ となっています。

### Sample Explanation 2

恷弌�､鰉襪┐誥�方双 $ B $, $ C $ として、箭えば肝があります�� - $ B\ =\ (0,\ 1,\ 2,\ 4) $ - $ C\ =\ (5,\ 3,\ 1,\ 1) $

### Sample Explanation 3

恷弌�､鰉襪┐誥�方双 $ B $, $ C $ として、箭えば肝があります�� - $ B\ =\ (-3) $ - $ C\ =\ (-7) $

