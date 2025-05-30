## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc057/tasks/abc057_d

$ N $ 個の品物が与えられます。  
 $ i $ 番目の品物の価値は $ v_i\ (1≦i≦N) $ です。  
 これらの品物から、$ A $ 個以上、$ B $ 個以下を選ばなければなりません。  
 この制約下において、選んだ品物の価値の平均の最大値を求めてください。  
 また、選んだ品物の平均が最大となるような品物の選び方が何通りあるかを求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ A $ $ B $ $ v_1 $ $ v_2 $ $ ... $ $ v_N $

## 输出格式
解答を $ 2 $ 行に出力せよ。  
 $ 1 $ 行目には、選んだ品物の価値の平均の最大値を出力せよ。絶対誤差または相対誤差が $ 10^{−6} $ 以下ならば正解となる。  
 $ 2 $ 行目には、選んだ品物の平均が最大となるような品物の選び方の数を出力せよ。

## 题目大意
有n个数，可以选取最少A个最多B个，使得所选的数的平均值最大。求可能的最大平均值 和 在平均值最大的情况下的方案数

```input1
5 2 2
1 2 3 4 5
```

```output1
4.500000
1
```

```input2
4 2 3
10 20 10 10
```

```output2
15.000000
3
```

```input3
5 1 5
1000000000000000 999999999999999 999999999999998 999999999999997 999999999999996
```

```output3
1000000000000000.000000
1
```

```input4
50 1 50
1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1
```

```output4
1.000000
1125899906842623
```

## 提示
### 制約

- $ 1≦N≦50 $
- $ 1≦A≦B≦N $
- $ 1≦v_i≦10^{15} $
- $ v_i $ は全て整数である。

### Sample Explanation 1

$ 4 $ 番目の品物と $ 5 $ 番目の品物を選ぶと価値の平均が最大となるため、出力の $ 1 $ 行目は $ 4.5 $ です。 また、それ以外の品物の選び方で価値の平均が $ 4.5 $ になるものはないため、出力の $ 2 $ 行目は $ 1 $ です。

### Sample Explanation 2

価値の平均が最大となる品物の選び方は複数存在することがあります。

