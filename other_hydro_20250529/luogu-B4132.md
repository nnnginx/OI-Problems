## 题目背景
本题有可能是假题，仅供参考。

## 题目描述
有 $n$ 个单词，每个单词由 $2$ 个小写字母组成，并约定第 $1$ 个单词为龙头。接龙的方法为：前一单词的第 $2$ 个字母和后一个单词的第 $1$ 个字母相同。**一个单词只能用一次。**

程序要求给出各个单词后，求出最长龙的长度。

## 输入格式
第一行一个整数，表示 $n$。

接下来 $n$ 行，每行有 $2$ 个小写字母，表示一个单词 $s_i$（单词字母间无空格）。

## 输出格式
一行一个整数，表示最长龙的长度。

```input1
7
aa
ac
ab
ef
bh
hk
cd
```

```output1
4
```

```input2
8
gd
bd
ea
ab
fd
be
df
be
```

```output2
6
```

## 提示
### 样例 $\textbf 1$ 解释
可以接龙的方法有：
- $\tt aa-ac-cd$，长度为 3；
- $\tt aa-ab-bh-hk$，长度为 4。
### 数据范围
$1\le n\le50$。

