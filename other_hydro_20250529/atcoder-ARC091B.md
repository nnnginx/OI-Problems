## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc090/tasks/arc091_b

高橋君は、$ N $ 以下の正の整数の $ 2 $ つ組 $ (a,b) $ を持っていましたが、忘れてしまいました。 高橋君は、$ a $ を $ b $ で割ったあまりが $ K $ 以上であったことを覚えています。 高橋君が持っていた組としてあるうるものの個数を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $

## 输出格式
高橋君が持っていた組としてあるうるものの個数を出力せよ。

## 题目大意
请求出有序正整数对 $(a,b)$ 的个数。每个对需要满足 $1\le a,b\le N$ ，且 $a\bmod b\ge K$ 。   

限制：$1\le N\le 10^5,0\le K<N$

```input1
5 2
```

```output1
7
```

```input2
10 0
```

```output2
100
```

```input3
31415 9265
```

```output3
287927211
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 10^5 $
- $ 0\ \leq\ K\ \leq\ N-1 $
- 入力は全て整数である

### Sample Explanation 1

ありうる組は、$ (2,3),(5,3),(2,4),(3,4),(2,5),(3,5),(4,5) $ の $ 7 $ 組です。

