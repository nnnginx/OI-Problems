## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/abc188/tasks/abc188_b

$ 2 $ つの $ N $ 肝圷ベクトル $ A\ =\ (A_1,\ A_2,\ A_3,\ \dots,\ A_N),\ B\ =\ (B_1,\ B_2,\ B_3,\ \dots,\ B_N) $ が嚥えられます。  
 $ A $ と $ B $ の坪�eが $ 0 $ かどうかを登協してください。  
 すなわち、$ A_1B_1\ +\ A_2B_2\ +\ A_3B_3\ +\ \dots\ +\ A_NB_N\ =\ 0 $ かどうかを登協してください。

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられる。

> $ N $ $ A_1 $ $ A_2 $ $ A_3 $ $ \dots $ $ A_N $ $ B_1 $ $ B_2 $ $ B_3 $ $ \dots $ $ B_N $

## 補竃鯉塀
$ A $ と $ B $ の坪�eが $ 0 $ ならば `Yes` を、$ 0 $ でないならば `No` を竃薦せよ。

## 籾朕寄吭
公協曾倖海業葎 $n$ 議方怏��$A$ 才 $B$。

飛 $A_1 \times B_1 + A_2 \times B_2 +\cdots+A_n \times B_n = 0$ ��夸補竃 ``Yes``��倦夸補竃 ``No``。

```input1
2
-3 6
4 2
```

```output1
Yes
```

```input2
2
4 5
-1 -3
```

```output2
No
```

```input3
3
1 3 5
3 -6 3
```

```output3
Yes
```

## 戻幣
### 崙�s

- $ 1\ \le\ N\ \le\ 100000 $
- $ -100\ \le\ A_i\ \le\ 100 $
- $ -100\ \le\ B_i\ \le\ 100 $
- 秘薦に根まれる�､枠�て屁方である

### Sample Explanation 1

$ A $ と $ B $ の坪�eは $ (-3)\ \times\ 4\ +\ 6\ \times\ 2\ =\ 0 $ です。

### Sample Explanation 2

$ A $ と $ B $ の坪�eは $ 4\ \times\ (-1)\ +\ 5\ \times\ (-3)\ =\ -19 $ です。

### Sample Explanation 3

$ A $ と $ B $ の坪�eは $ 1\ \times\ 3\ +\ 3\ \times\ (-6)\ +\ 5\ \times\ 3\ =\ 0 $ です。

