## 题目描述

给定 $n$ 个字符串，从之中选出若干个字符串，最大化这些字符串的最长公共前缀长度与选出字符串个数的乘积。

## 输入格式

第一行一个整数 $n$，接下来 $n$ 行每行一个字符串，不保证字符串中没有空格。

## 输出格式

一行一个整数表示最大答案。

```input1
7
Jora de Sus
Orhei
Jora de Mijloc
Joreni
Jora de Jos
Japca
Orheiul Vechi
```

```output1
24
```

## 数据规模与约定

对于 $100\%$ 的数据，$2 \le n \le 10 ^ 6$，单个字符串长度不超过 $2 \times 10 ^ 4$，输入文件大小不超过 10 $\text{Mib}$。