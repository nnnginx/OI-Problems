## 题目描述
给定长度为 $N$ 的字符串 $S$，仅包含 $\tt{J,O,I}$，三种字符，对字符串的每一个字符 $c$ 你需要做如下操作。

- 如果 $c=\tt{J}$，那么 $c'$ 为 $\tt{O}$
- 如果 $c=\tt{O}$，那么 $c'$ 为 $\tt{I}$
- 如果 $c=\tt{I}$，那么 $c'$ 为 $\tt{J}$
- 然后令 $c\leftarrow c'$。

求操作完的字符串。

## 输入格式
第一行一个正整数 $N$。

第二行一个长度为 $N$ 的字符串 $S$。


## 输出格式
一行一个字符串表示答案。

```input1
3
JOI
```

```output1
OIJ
```

```input2
10
JOIOOJOOOJ
```

```output2
OIJIIOIIIO
```

## 提示
### 样例解释

执行操作以后 $\tt{JOI}$ 变为 $\tt{OIJ}$，$\tt{JOIOOJOOOJ}$ 变为 $\tt{OIJIIOIIIO}$。

### 数据范围 

$1\leq N\leq 100$，保证 $S$ 中只含 $\tt{J,O,I}$ 三种字符。

