## 题目描述
 
受校门外的树这道经典问题的启发，A 君根据基本的离散数学的知识，抽象出 $5$ 种运算维护集合 $S$（$S$ 初始为空）并最终输出 $S$。现在，请你完成这道校门外的树之难度增强版——校门外的区间。
 

5种运算如下：

* `U T`: $S = S \cup T$
* `I T`: $S = S \cap T$
* `D T`: $S = S - T$
* `C T`: $S = T - S$
* `S T`: $S = S \oplus T$


基本集合运算如下：

* $A \cup B = \{x \mid x \in A \vee x \in B \}$
* $A \cap B = \{x \mid x \in A \wedge x \in B \}$
* $A - B = \{x \mid x \in A \wedge x \not\in B \}$
* $A \oplus B = (A - B) \cup (B - A)$
  
## 输入格式

输入共 $m$ 行。

每行的格式为 `X T`，用一个空格隔开，$X$ 表示运算的种类，$T$ 为一个区间（区间用 `(a,b)`, `(a,b]`, `[a,b)`, `[a,b]` 表示）。

## 输出格式
 
共一行，即集合 $S$，<font color=red>每个区间后面带一个空格</font>。若 $S$ 为空则输出 `empty set`。

```input1
U [1,5]
D [3,3]
S [2,4]
C (1,5)
I (2,3]
```

```output1
(2,3)
```

## 数据规模与约定

* 对于 $100\%$ 的数据，$0 \leq a \leq b \leq 65535$，$1 \leq m \leq 7 \times 10^4$。

## 题目来源

线段树