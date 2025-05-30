## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc140/tasks/abc140_d

東西一列に $ N $ 人の人が並んでいます。

各人の状態を表す長さ $ N $ の文字列 $ S $ が与えられます。 西から $ i $ 番目の人は、文字列 $ S $ の $ i $ 文字目が `L` ならば西を、`R` ならば東を向いています。

どの人も、目の前の人が自分と同じ方向を向いていれば幸福です。 ただし、目の前に人が居ない場合、幸福ではありません。

あなたは、以下の操作を $ 0 $ 回以上 $ K $ 回以下の好きな回数だけ行います。

操作: $ 1\ \leq\ l\ \leq\ r\ \leq\ N $ を満たす整数 $ l,\ r $ を選ぶ。西から $ l,\ l+1,\ ...,\ r $ 番目の人の列を $ 180 $ 度回転する。すなわち、$ i\ =\ 0,\ 1,\ ...,\ r-l $ について、西から $ l\ +\ i $ 番目の人は操作後には西から $ r\ -\ i $ 番目に移動し、元々西を向いていれば東を、東を向いていれば西を向く。

幸福である人は最大で何人にできるでしょうか。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ S $

## 输出格式
$ K $ 回以下の操作後に幸福である人数の最大値を出力せよ。

## 题目大意
### 题目描述
有 $N$ 个人从东向西排成一排，每个人的状态用一个字符串 $S$ 表示，第i个字符 $s_i$

 表示从西边数起第 $i$ 个人的朝向```L```
表示面朝西， ```R``` 表示面朝东。

对于队伍中的每个人，如果自己面前的人的朝向和自己一样，那么这个人就会感到幸福。如果面前的人朝向和自己不一样，或者面前没有人，这个人就感到不幸福。

你可以进行以下操作最多 $K$ 次（也可以一次都不进行）：

选择整数$l,r（1≤l≤r≤N）$，让从西边数起第 $l,l+1,⋯,r$ 个人转身180度。

经过最多 $K$ 次操作后，感到幸福的人最多有多少人？
### 输入格式
第1行，2个正整数 $N,K$。

第2行，一个字符串 $S$ 。
### 输出格式
一行一个正数表示答案

```input1
6 1
LRLRRL
```

```output1
3
```

```input2
13 3
LRRLRLRRLRLLR
```

```output2
9
```

```input3
10 1
LLLLLRRRRR
```

```output3
9
```

```input4
9 2
RRRLRLRLL
```

```output4
7
```

## 提示
### 制約

- $ N $ は $ 1\ \leq\ N\ \leq\ 10^5 $ を満たす整数である。
- $ K $ は $ 1\ \leq\ K\ \leq\ 10^5 $ を満たす整数である。
- $ |S|\ =\ N $
- $ S $ の各文字は `L` または `R` である。

### Sample Explanation 1

$ (l,\ r)\ =\ (2,\ 5) $ と選べば `LLLRLL` となり、西から $ 2,\ 3,\ 6 $ 番目の人が幸福です。

