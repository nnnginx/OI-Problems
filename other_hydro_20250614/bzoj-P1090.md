## 题目描述

折叠的定义如下：

1. 一个字符串可以看成它自身的折叠。记作 $S=S$ ． 
2. $X(S)$ 是 $X(X>1)$ 个 $S$ 连接在一起的串的折叠。记作 $X(S) = SSSS…S$（$X$ 个 $S$）。
3. 如果 $A = A',B = B'$，则 $AB = A'B'$ 。例如：因为 $\mathtt{3(A) = AAA,2(B) = BB}$， 所以 $\mathtt{3(A)C2(B) = AAACBB}$，而 $\mathtt{2(3(A)C)2(B) = AAACAAACBB}$．

给一个字符串，求它的最短折叠。例如 $\mathtt{AAAAAAAAAABABABCCD}$ 的最短折叠为：$\mathtt{9(A)3(AB)CCD}$。

## 输入格式

仅一行，即字符串 $S$。

## 输出格式

仅一行，即最短的折叠长度。

```input1
NEERCYESYESYESNEERCYESYESYES
```

```output1
14
```

## 数据规模与约定

$S$ 的长度保证不超过 $100$．

## 提示

一个最短的折叠为：$\mathtt{2(NEERC3(YES))}$。