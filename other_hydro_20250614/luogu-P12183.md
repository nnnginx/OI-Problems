## 题目背景
The English statement is provided [here](https://www.luogu.com.cn/problem/U495394). **You must submit your solution only at the Chinese version.**

## 题目描述
给定正整数 $n$，构造 $n$ 个正整数 $a_1,a_2,\cdots,a_n$，使得 $\displaystyle\sum_{i=1}^n a_i=\operatorname{lcm}(a_1,a_2,\cdots,a_n)$（其中 $\operatorname{lcm}$ 为最小公倍数运算），并且这组数的极差是所有构造的极差中最小的。极差指一组数当中的最大值减最小值。

**并且，你构造的这 $n$ 个数的最小公倍数不得超过 $10^{12}$。否则，SPJ 可能出现未定义行为。**

## 输入格式
一个整数 $n$。

## 输出格式
$n$ 个正整数，表示你构造的答案（你可以用任意顺序输出），并用空格分隔。

**请勿在行末输出多余的空格，否则你的输出可能被判为错误。**

```input1
3
```

```output1
1 2 3
```

## 提示
#### 样例说明

容易证明，$n=3$ 时不存在极差小于 $2$ 的构造方案，因此输出一组极差为 $2$ 的构造符合题意。另外，`1 3 2`，`3 2 1` 等也符合条件。

#### 数据范围

$3\le n\le 5\times 10^6$。

