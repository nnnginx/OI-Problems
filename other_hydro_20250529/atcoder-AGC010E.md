## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc010/tasks/agc010_e

黒板に $ N $ 個の整数が書かれています。$ i $ 番目の整数は $ A_i $ です。

高橋君と青木君は以下の手順でこれらの数を一列に並べることにしました。

- 最初に、高橋君が好きな順に一列に並べる。
- 次に、青木君が隣り合う $ 2 $ つの数を選んで入れ替えることを好きな回数だけ繰り返す。  
   ただし、入れ替える $ 2 $ 数は互いに素でなければならない。

高橋君は最終的な並びが辞書順最小となるように、青木君は最終的な並びが辞書順最大となるように最適に行動するとしたとき、 最終的な数列を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ … $ A_N $

## 输出格式
最終的な数列を一行に出力せよ。

## 题目大意
有一个 $n$ 个数组成的序列 $a_i$。

高桥君会把整个序列任意排列，然后青木君可以进行任意次操作，每次选择两个相邻的互质的数交换位置。

高桥君希望最终序列的字典序尽量小，而青木君希望字典序尽量大。求最终序列。

```input1
5
1 2 3 4 5
```

```output1
5 3 2 4 1
```

```input2
4
2 3 4 6
```

```output2
2 4 6 3
```

## 提示
### 制約

- $ 1\ ≦\ N\ ≦\ 2000 $
- $ 1\ ≦\ A_i\ ≦\ 10^8 $

### Sample Explanation 1

高橋君は与えられた数を $ (1,2,3,4,5) $ という順番で並べれば、青木君が最適に動かしても $ (5,3,2,4,1) $ となります。

