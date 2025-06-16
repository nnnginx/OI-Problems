## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc220/tasks/abc220_a

$ A $ 以上 $ B $ 以下であるような $ C $ の倍数を、$ 1 $ つ出力してください。

条件を満たす数が存在しない場合は `-1` を出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ A $ $ B $ $ C $

## 输出格式
答えを出力せよ。  
 条件を満たす数が存在しない場合は `-1` を出力せよ。

## 题目大意
输出一个数 $k$ 满足 $k \in [a,b],k \bmod c = 0$。

若没有该数字，输出 `-1`。

Translated by ShanCreeper.

```input1
123 456 100
```

```output1
200
```

```input2
630 940 314
```

```output2
-1
```

## 提示
### 制約

- $ 1\ \leq\ A\ \leq\ B\ \leq\ 1000 $
- $ 1\ \leq\ C\ \leq\ 1000 $
- 入力は全て整数

### Sample Explanation 1

`300` や `400` も正解です。

