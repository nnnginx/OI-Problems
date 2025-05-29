## 题目描述
[problemUrl]: https://atcoder.jp/contests/s8pc-4/tasks/s8pc_4_c



## 输入格式
入力は、次の形式で与えられる。

> $ n $ $ m $ $ q $ $ a_1 $ $ a_2 $ ... $ a_q $

## 输出格式
連結な部分の個数を1行に出力しなさい。

```input1
7 7 3
1 3 5
```

```output1
4
```

```input2
10 14 8
5 6 7 8 9 10 11 12
```

```output2
10
```

## 提示
### 制約

- $ n $ ≦ $ 10^{12} $
- $ 7n $ は $ m $ で割り切れる。
- 1 ≦ $ q $ ≦ $ m $ ≦ $ 10^5 $
- $ 0 $ ≦ $ a_1 $ a\_2 a\_q

### 得点

 小課題1 \[$ 100 $ 点\]

- $ n $ ≦ $ 100000 $.
 
 小課題2 \[$ 90 $ 点\]   
- $ m $ は $ 7 $ の倍数
- $ a_{i\ +\ 1}\ -\ a_i\ =\ 1 $.
 
 小課題3 \[$ 200 $ 点\]   
- $ m $ は $ 7 $ の倍数
 
 小課題4 \[$ 110 $ 点\]   
- 追加の制約はない。

### Sample Explanation 1

次のようなカレンダーになる。よって、連結な部分の個数は $ 4 $ となる。 !\[\](https://atcoder.jp/img/s8pc-4/b7ae283b5c0a566376d05aeff63b100a.png)

### Sample Explanation 2

次のようなカレンダーになる。よって、連結な部分の個数は 14 $ 10 $ (2020/8/08 訂正) となる。 !\[\](https://atcoder.jp/img/s8pc-4/42a03c02d737a1c97005360832707eaa.png)

