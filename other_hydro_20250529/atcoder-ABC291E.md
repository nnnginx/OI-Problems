## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc291/tasks/abc291_e

$ 1,\ldots,N $ の並び替えである長さ $ N $ の数列 $ A=(A_1,\ldots,A_N) $ があります。

あなたは $ A $ を知りませんが、$ M $ 個の整数の組 $ (X_i,Y_i) $ について、$ A_{X_i}\ <\ A_{Y_i} $ が成り立つことを知っています。

$ A $ を一意に特定できるかどうか判定し、できるなら $ A $ を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ X_1 $ $ Y_1 $ $ \vdots $ $ X_M $ $ Y_M $

## 输出格式
$ A $ を一意に特定できるとき、1行目に `Yes` と出力し、2行目に $ A_1,\ldots,A_N $ をこの順に空白区切りで出力せよ。

$ A $ を一意に特定できないとき、`No` とのみ出力せよ。

## 题目大意
有一个 $1\sim N$ 的排列 $A_1,\cdots,A_N$。  
给定 $M$ 组关系 $(X_i,Y_i)$，每组关系表示 $A_{X_i}<A_{Y_i}$。  
求出唯一一组合法的 $A$。如果答案不唯一，仅输出 `No`；否则输出 `Yes` 和求出的 $A$。

```input1
3 2
3 1
2 3
```

```output1
Yes
3 1 2
```

```input2
3 2
3 1
3 2
```

```output2
No
```

```input3
4 6
1 2
1 2
2 3
2 3
3 4
3 4
```

```output3
Yes
1 2 3 4
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 2\times\ 10^5 $
- $ 1\ \leq\ M\ \leq\ 2\times\ 10^5 $
- $ 1\leq\ X_i,Y_i\ \leq\ N $
- 入力は全て整数である
- 入力に矛盾しない $ A $ が存在する

### Sample Explanation 1

$ A=(3,1,2) $ であると一意に特定できます。

### Sample Explanation 2

$ A $ として $ (2,3,1),(3,2,1) $ の $ 2 $ 通りが考えられます。

