## 题目描述

定义函数 $ \text{H}(s) $其中 $s$ 为一个二进制数，返回 $s$ 转成字符串以后，把所有的「1」变成「10」，「0」变成「1」。比如 $\text{H}(\texttt{1001})=\texttt{101110}$。特殊地，$\text{H}("")="",\text{H}_m(s)=\text{H}(\text{H}(\text{H}(\dots \text{H}(s))))\dots)$，即自我运算 $m$ 次。特别的，$\text{H}_0(s)=s$。

输入 $n$ 个数 $T_1 \dots T_n$ 判断 $\text{H}_{T_1}(\texttt{0}),\text{H}_{T_2}(\texttt{0}), \dots ,\text{H}_{T_n}(\texttt{0})$ 是否是 $\text{H}_m(\texttt{0})$ 的子串，$m$ 为任意正整数。

## 输入格式

第一行正整数 $T$ 表示数据组数。每组数据包括：第一行 $n$。

第二行 $n$ 个非负整数 $T_{1 \dots n}$。

## 输出格式

$N$ 行，每行一个字符串 `TAK`/`NIE` 表示是/否。


```input1
2
2
1 2
2
2 0
```

```output1
TAK
NIE
```

## 数据规模与约定

$1 \le T \le 13$

$1 \le n \le 10^5$

$\sum T \le 10^7$