## 题目背景

你还好吗

你自由地在天空翱翔了吗

你有使出很厉害的魔法吗

这些全都是梦里限定品喔

——[ドリームレス・ドリームス 无梦之梦（不插电）](https://music.163.com/#/song?id=529391584)

## 题目描述

mikage 有两个长度为 $n$ 且仅包含 `#` 和小写字母的字符串 $a,b$。

这两个字符串总共包含 $m$ 个 `#`，mikage 打算执行 $m$ 次操作，用小写字母把两个字符串中所有的 `#` 都替换掉。
  
对于第 $i$ 次操作，他要在 $a,b$ 中选择一个字符串，将这个字符串中从左向右数第一个 `#` 替换为第 $(i-1) \bmod 26 +1$ 个小写字母。**她不能选择不包含 `#` 的字符串。**

mikage 想最小化执行完 $m$ 次操作后的字符串 $a$ 的字典序。

## 输入格式

第一行输入两个正整数 $n,m$。

第二行输入一个长度为 $n$ 的字符串 $a$。

第三行输入一个长度为 $n$ 的字符串 $b$。

## 输出格式

输出一行一个字符串，表示执行 $m$ 次操作后能够得到的字典序最小的 $a$。



```input1
8 2
th#nkyou
#estwish
```



```output1
thankyou
```

## 样例 1 解释

第一次操作选择字符串 $a$，将 $a$ 中的 `#` 替换为第 $(1-1) \bmod 26+1=1$ 个小写字母，即 `a`；第二次操作选择字符串 $b$，将 $b$ 中的 `#` 替换为第 $(2-1) \bmod 26+1=2$ 个小写字母，即 `b`。最终的字符串 $a$ 即为 `thankyou`，可以证明这是执行 $m$ 次操作后能得到的字典序最小的 $a$。

## 数据范围

对于所有测试数据，$1 \leq n \leq 10^5$，$1 \leq m \leq 2n$，字符串 $a,b$ 仅包含字符 `#` 和小写字母。



