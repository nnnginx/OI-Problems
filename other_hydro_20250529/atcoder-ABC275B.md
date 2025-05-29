## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc275/tasks/abc275_b

非負整数 $ A,B,C,D,E,F $ があり、$ A\times\ B\times\ C\geq\ D\times\ E\times\ F $ をみたしています。  
 $ (A\times\ B\times\ C)-(D\times\ E\times\ F) $ の値を $ 998244353 $ で割った余りを求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ A $ $ B $ $ C $ $ D $ $ E $ $ F $

## 输出格式
$ (A\times\ B\times\ C)-(D\times\ E\times\ F) $ を $ 998244353 $ で割った余りを整数で出力せよ。

## 题目大意
输入 $A,B,C,D,E,F(0\le A,B,C,D,E,F\le10^{18})$，输出 $(A\times B\times C)-(D\times E \times F) \mod 998244353$

```input1
2 3 5 1 2 4
```

```output1
22
```

```input2
1 1 1000000000 0 0 0
```

```output2
1755647
```

```input3
1000000000000000000 1000000000000000000 1000000000000000000 1000000000000000000 1000000000000000000 1000000000000000000
```

```output3
0
```

## 提示
### 制約

- $ 0\leq\ A,B,C,D,E,F\leq\ 10^{18} $
- $ A\times\ B\times\ C\geq\ D\times\ E\times\ F $
- $ A,B,C,D,E,F $ は整数

### Sample Explanation 1

$ A\times\ B\times\ C=2\times\ 3\times\ 5=30 $, $ D\times\ E\times\ F=1\times\ 2\times\ 4=8 $ より、 $ (A\times\ B\times\ C)-(D\times\ E\times\ F)=22 $ であり、これを $ 998244353 $ で割った余りである $ 22 $ を出力します。

### Sample Explanation 2

$ A\times\ B\times\ C=1000000000 $, $ D\times\ E\times\ F=0 $ より、 $ (A\times\ B\times\ C)-(D\times\ E\times\ F)=1000000000 $ であり、これを $ 998244353 $ で割った余りである $ 1755647 $ を出力します。

### Sample Explanation 3

$ (A\times\ B\times\ C)-(D\times\ E\times\ F)=0 $ であり、これを $ 998244353 $ で割った余りである $ 0 $ を出力します。

