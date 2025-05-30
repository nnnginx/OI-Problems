## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc064/tasks/arc064_d

高橋君と青木君が協力して数列を作ることになりました。

まず、高橋君が次の条件をすべて満たす数列 $ a $ を用意します。

- $ a $ は長さ $ N $ である。
- $ a $ の各要素は $ 1 $ 以上 $ K $ 以下の整数である。
- $ a $ は回文である。 すなわち、$ a $ を逆順にした数列は元の $ a $ と一致する。

次に、青木君が次の操作を好きな回数だけ繰り返します。

- $ a $ の先頭要素を末尾へ移動する。

以上の手続きにより、最終的な $ a $ が得られます。

最終的な $ a $ として考えられるものは何通りあるでしょうか？ $ 10^9+7 $ で割った余りを求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $

## 输出格式
最終的な $ a $ として考えられるものは何通りあるか？ $ 10^9+7 $ で割った余りを出力せよ。

## 题目大意
高桥和青木想要一起造一个数列。

首先，高桥会造出一个满足以下条件的数列$a$：

* $a$的长度为$N$。
* $a$中的所有元素都是一个$[1,K]$内的整数。
* $a$是一个回文串。

然后，青木会进行任意多次以下的操作：

* 把$a$中的第一个元素移到最后。

经过这些步骤，一共可以得到多少种不同的数列$a$呢？答案对1e9+7取模。

```input1
4 2
```

```output1
6
```

```input2
1 10
```

```output2
10
```

```input3
6 3
```

```output3
75
```

```input4
1000000000 1000000000
```

```output4
875699961
```

## 提示
### 制約

- $ 1\ <\ =N\ <\ =10^9 $
- $ 1\ <\ =K\ <\ =10^9 $

### Sample Explanation 1

次の $ 6 $ 通りです。 - $ (1,\ 1,\ 1,\ 1) $ - $ (1,\ 1,\ 2,\ 2) $ - $ (1,\ 2,\ 2,\ 1) $ - $ (2,\ 2,\ 1,\ 1) $ - $ (2,\ 1,\ 1,\ 2) $ - $ (2,\ 2,\ 2,\ 2) $

