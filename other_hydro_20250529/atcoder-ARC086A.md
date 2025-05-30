## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc081/tasks/arc086_a

高橋君は，$ N $ 個のボールを持っています． 最初，$ i $ 番目のボールには，整数 $ A_i $ が書かれています．

高橋君は，いくつかのボールに書かれている整数を書き換えて，$ N $ 個のボールに書かれている整数が $ K $ 種類以下になるようにしたいです．

高橋君は，少なくとも何個のボールの整数を書き換える必要があるでしょうか？

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ A_1 $ $ A_2 $ ... $ A_N $

## 输出格式
高橋君が，少なくとも何個のボールの整数を書き換える必要があるかを出力せよ．

## 题目大意


有N个球，第I个球上写入整数Ai。

改变一些球的数字，以便在N个球上最多写入K个不同的数。

找到所需重写的最小球数。


感谢@chengni 提供的翻译

```input1
5 2
1 1 2 2 5
```

```output1
1
```

```input2
4 4
1 1 2 2
```

```output2
0
```

```input3
10 3
5 1 3 2 4 1 1 2 3 4
```

```output3
3
```

## 提示
### 制約

- $ 1\ \leq\ K\ \leq\ N\ \leq\ 200000 $
- $ 1\ \leq\ A_i\ \leq\ N $
- 与えられる数値はすべて整数

### Sample Explanation 1

例えば，$ 5 $ 番目のボールに書かれている整数を $ 2 $ に変更すると，ボールに書かれている整数は $ 1,\ 2 $ の $ 2 $ 種類となります． 一方，まったく書き換えを行わずに，ボールに書かれている整数の種類数を $ 2 $ 以下にすることはできないので，$ 1 $ を出力します．

### Sample Explanation 2

最初，ボールに書かれている整数の種類数は $ 2 $ なので，まったく書き換えを行う必要はありません．

