## 题目描述
小威正在学习字符串相关的内容，今天，他开始学习 KMP 算法。

正好，小海精通 KMP 算法，向小威讲述了算法流程，并向小威提出了一个问题：

小海给了小威一个长度为 $n$ 的字符串 $s$，定义一个前缀 $s_{1:i}$ 的价值 
$$v_i = i \oplus \operatorname{len}(\operatorname{border}(s_{1:i}))$$ 
其中：
- $\oplus$ 表示按位异或；
- $\operatorname{border}(s)$ 表示 $s$ 中最长的前缀与后缀相同的子串，例如：$\operatorname{border}(abcda) = a$，$\operatorname{border}(aaa) = aa$；
- $\operatorname{len}(s)$ 表示 $s$ 的长度。

特别地，定义空串的价值 $v_0 = 0$。

小海告诉小威，如果要在 $s$ 中选择一个前缀 $t$，那同时要选择前缀 $\operatorname{border}(t)$，例如，如果小威选择了 $aaa$，那么小威需要同时选择 $aa, a, \varepsilon$，其中 $\varepsilon$ 表示空串。如此，小威选择了 $\{aaa, aa, a, \varepsilon\}$ 共 $4$ 个前缀。称这为一个前缀集合，前缀集合的价值为集合中所有前缀的价值之和。

对于一个字符串 $x$ 的前缀集合 $u$，和另一个字符串 $y$ 的前缀集合 $v$，设把它们合并后的前缀集合为 $\{u \cup v\} \setminus \{u \cap v\} \cup \{g(x, y)\}$。其中 $g(x, y)$ 表示 $x$ 和 $y$ 的最长公共 border。特别地，若 $x$ 属于 $y$ 的 前缀集合，则 $g(x,y) = x$。

例如，$u$ 为 $aaa$ 的前缀集合，$v$ 为 $aba$ 的前缀集合，则合并后为
$$\{\varepsilon, a, aa, aaa, aba\} \setminus \{\varepsilon, a\} \cup \{a\} = \{a, aa, aaa, aba\}$$

小海会问小威 $m$ 次，是否存在两个不同的前缀集合 $u$ 和 $v$，使得合并 $u$ 和 $v$ 后的价值之和为 $k$？


## 输入格式
第一行两个整数 $n, m$，含义如上所述。

第二行一个长度为 $n$ 的字符串 $s$，含义如上所述。

接下来 $m$ 行，每行一个整数 $k$，含义如上所述。

对于所有数据，满足：$1 \leq n\leq 3 \times 10^4$，$1 \leq m \leq 500$，$0 \leq k \leq 10^7$，$s$ 中仅包含小写英文字符。

## 输出格式
对于每次询问，输出一个字符串代表答案。如果存在输出 `Yes`，否则输出 `No`。

```input1
5 4
abcab
0
15
10
18

```

```output1
No
Yes
Yes
No

```

```input2
10 8
wlwlwlwlwl
0
14
1
9
6
2
2
14

```

```output2
No
No
Yes
Yes
No
Yes
Yes
No

```

