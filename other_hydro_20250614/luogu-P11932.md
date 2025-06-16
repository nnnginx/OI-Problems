## 题目背景
译自 [Natjecanje timova studenata informatičara hrvatskih sveučilišta](https://hsin.hr/studenti2024/) B.

## 题目描述
给定非负整数序列 $a,b,c$，长度分别为 $|a|,|b|,|c|$。这里序列下标是 **0-indexed** 的。

令 $l=\max\{a_i,b_i,c_i\}$。

找到任意一个 $\in [l+1,10^{19})$ 的正整数 $B$，使得 $\displaystyle \left(\sum_{0\le i\lt |a|} a_iB^i\right)\left(\sum_{0\le j\lt |b|} b_jB^j\right)=\sum_{0\le k\lt |c|} c_kB^k$ 成立。

数据保证，若存在正整数 $B\ge l+1$ 使得上式成立，则存在一个 $\in [l+1,10^{19})$ 的正整数 $B$ 使得上式成立。


## 输入格式
第一行，$|a|+1$ 个非负整数 $|a|,a_{|a|-1},a_{|a|-2},\ldots,a_0$。

第二行，$|b|+1$ 个非负整数 $|b|,b_{|b|-1},b_{|b|-2},\ldots,b_0$。

第一行，$|c|+1$ 个非负整数 $|c|,c_{|c|-1},c_{|c|-2},\ldots,c_0$。

**数据保证 $a_{|a|-1},b_{|b|-1},c_{|c|-1}\neq 0$。**


## 输出格式
如果存在 $\in [l+1,10^{19})$ 的 $B$，直接输出；

否则输出一行一个 $\texttt{impossible}。$


**数据保证，若存在正整数 $B\ge l+1$ 使得上式成立，则存在一个 $\in [l+1,10^{19})$ 的正整数 $B$ 使得上式成立。**

```input1
2 2 0
1 2
3 1 0 0
```

```output1
4
```

```input2
3 5 1 2
2 11 3
5 4 5 1 12 6
```

```output2
13
```

```input3
2 3 2
2 3 2
3 10 12 4
```

```output3
impossible
```

## 提示
- $1\le |a|,|b|,|c|\le 10^3$；
- $0\le a_i,b_i,c_i\le 2^{30}$；
- $a_{|a|-1},b_{|b-1|},c_{|c-1|}\neq 0$。
- 若存在正整数 $B\ge l+1$ 使得上式成立，则存在一个 $\in [l+1,10^{19})$ 的正整数 $B$ 使得上式成立。

