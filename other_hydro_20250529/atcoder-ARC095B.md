## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc094/tasks/arc095_b

$ n $ 個のものから順番を無視して $ r $ 個を選ぶ場合の数を $ {\rm\ comb}(n,r) $ と書くことにします。 $ n $ 個の非負の整数 $ a_1,\ a_2,\ ...,\ a_n $ から $ 2 $ つの数 $ a_i\ >\ a_j $ を $ {\rm\ comb}(a_i,a_j) $ が最大になるように選んで下さい。 最大になる組が複数ある場合、どれを選んでも構いません。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ n $ $ a_1 $ $ a_2 $ $ ... $ $ a_n $

## 输出格式
選んだ $ 2 $ つの数を空白区切りで降順に出力せよ。

## 题目大意
给定各数两两不相同的序列 $A$，请在其中找出两个数 $x,y$ 使得 $C_{x}^y$ 最大，并输出您选的 $x$ 与 $y$。

**所有正确答案都被判正确。**

```input1
5
6 9 4 2 11
```

```output1
11 6
```

```input2
2
100 0
```

```output2
100 0
```

## 提示
### 制約

- $ 2\ \leq\ n\ \leq\ 10^5 $
- $ 0\ \leq\ a_i\ \leq\ 10^9 $
- $ a_1,a_2,...,a_n $ は互いに相異なる
- 入力はすべて整数

### Sample Explanation 1

それぞれ計算すると - $ \rm{comb}(4,2)=6 $ - $ \rm{comb}(6,2)=15 $ - $ \rm{comb}(6,4)=15 $ - $ \rm{comb}(9,2)=36 $ - $ \rm{comb}(9,4)=126 $ - $ \rm{comb}(9,6)=84 $ - $ \rm{comb}(11,2)=55 $ - $ \rm{comb}(11,4)=330 $ - $ \rm{comb}(11,6)=462 $ - $ \rm{comb}(11,9)=55 $ となるため、$ 11 $ と $ 6 $ を出力します。

