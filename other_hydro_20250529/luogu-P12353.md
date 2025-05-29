## 题目背景
![](https://cdn.luogu.com.cn/upload/image_hosting/7mafbnqx.png?x-oss-process=image/resize,m_lfit,h_340,w_450)

（图片来自 Arcaea 曲绘，如有侵权请联系出题人删除。）

> How do you know you are not a Program?

## 题目描述
小 N 有两个 $\tt01$ 串 $S$ 和 $T$，其长度分别为 $N$ 和 $N+1$。你可以对 $T$ 进行一些修改。

- 选定 $1\leq i \leq |T|$，删除 $T_i$，其余字符下标左移。
- 选定 $1\leq l\leq r\leq |T|$，对于所有 $l\leq i\leq r$ 且 $(l+i)\equiv 0\pmod 2$ 的 $i$ 执行 $T_i\gets T_i\oplus 1$。

小 N 想使得 $T = S$，但是她非常懒，所以你需要最小化操作次数。

**注意：你只需要输出这个最小化的操作次数即可，而无需给出构造。**

## 输入格式
**本题单测试数据内含有多组输入。**

第一行一个正整数 $K$ 表示数据组数。

接下来每组测试数据第一行一个正整数 $N$ 含义如题面所述。

第二行为 $\tt01$ 串 $T$，由 $N+1$ 个字符（$\tt0$ 或 $\tt1$）构成，注意字符之间没有空格。

第二行为 $\tt01$ 串 $S$，由 $N$ 个字符（$\tt0$ 或 $\tt1$）构成，注意字符之间没有空格。

## 输出格式
共 $K$ 行，对于每组测试数据输出一行一个数表示答案。

```input1
1
4
10101
1111
```

```output1
2
```

```input2
3
1
11
1
3
1010
010
7
10110110
0001111
```

```output2
1
1
2
```

## 提示
### 样例解释 1 
- $1\textbf 01\textbf 01\to 1\textbf11\textbf11$
- $111\underline{1}\to 111$

使用 $2$ 次步骤。

### 数据规模与约定

**本题采用捆绑测试。**

- Subtask 0 (15pts)：$1\leq \sum N\leq 10$。
- Subtask 1 (35pts)：$1\leq \sum N\leq 10^3$。
- Subtask 2 (50pts)：无特殊限制。

对于所有数据，$1\leq K\leq 1000$，$1\leq \sum N\leq 10^6$，$1\leq N\le 10^6$。

