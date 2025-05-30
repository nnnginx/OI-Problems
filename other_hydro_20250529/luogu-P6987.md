## 题目描述


NEERC featured a number of problems about cactuses -- connected undirected graphs in which every edge belongs to at most one simple cycle. Intuitively, cactus is a generalization of a tree where some cycles are allowed.

In $2005$ , the first year where a problem about cactuses appeared, the problem was called simply `Cactus`. In $2007$ it was `Cactus Reloaded`, in $2010$ it was called `Cactus Revolution`, and in $2013$ it was called `Cactus Automorphisms`. Here is an example of cactus that was used in those problems:

![](/upload/images2/cactus.png)

For four years judges had to generate test files for cactuses with thousands of vertices. Of course, a number of test generators of ever-increasing complexity were built, culminating with a domain-specific language called CGL -- Cactus Generator Language. CGL can compactly define a big cactus for purposes of a test. In this problem you have to parse a simplified version of this language, which we call SCGL -- Simple Cactus Generator Language, and output a resulting cactus.

A cactus has to be output by listing the minimal set of edge-distinct paths that cover the whole graph.

The syntax of SCGL cactus definition is represented by the graph non-terminal in the grammar that is given below using the Extended Backus-Naur Form:

graph $=$ `c`

$|$ `c(` list `)`

$|$ `loop(` list `)`

$|$ `t(` list `)`

list $=$ graph ${$ `,` graph $}$

$|$ (number $|$ range $|$ variable ) $[$ `,` graph $]$

number $=$ nzdig ${$ `0` $|$ nzdig $}$

nzdig $=$ `1` $|$ `2` $| \cdots |$ `8` $|$ `9`

range $=$ `range(` variable `,` numvar `,` numvar `)`

variable $=$ `A` $|$ `B` $| \cdots |$ `Y` $|$ `Z`

numvar $=$ number $|$ variable

A graph production rule denotes a graph with two labeled vertices -- the first and the last. Graphs definition rules have the following semantics:

The basic building block $c$ denotes a graph with just two vertices (one is the first and the other one is the last) and one edge.

The $c(σ)$ rule connects a specified list of graphs $σ$ from left to right into a chain, merging the last vertex of the first graph in the list with the first vertex of the second graph in the list, the last vertex of the second graph with the first of the third one, and so on. The resulting graph's first vertex is the first vertex of the first graph in the list, and the resulting graph's last vertex is the last vertex of the last graph in the list.

The $loo_p(σ)$ rule connects a specified list of graphs $σ$ from left to right, merging the last vertex of the first graph in the list with the first vertex of the second graph in the list, and so on like in $c(σ),$ while the last vertex of the last graph in the list is merged with the first vertex of the first graph in the list to form a loop. The resulting graph's first and last vertices are the first and the last vertices of the first graph in the list. Loop can be applied only to lists with more than one graph.

The $t(σ)$ rule connects a specified list of graphs $σ,$ merging their first vertices. The resulting graph's first and last vertices are the first and the last vertices of the first graph in the list.

The list of graphs is either specified explicitly, by a comma-separated list, or using a list repetition with a number, a range, or a variable, optionally followed by a comma and a graph. When a graph is not explicitly specified in a list repetition, then the given graph is assumed to be $c$ .

The simplest list repetition is defined using a number non-terminal. It denotes a list of graphs with the specified integer number of copies of the given graph.

A range list repetition is defined by $range(ν, α, β)$ rule which has three components -- a variable $ν,$ and numbers $α$ and $β.$ If $ξ$ character sequence is a graph, then $c|loo_p|t(range(ν, α, β), ξ)$ are called rangeenabled rules and the variable $ν$ is called a bound variable in $ξ.$ In the context of a range-enabled rule, $ξ$ is repeated $|β − α| + 1$ times to form a list. Every occurrence of variable $ν$ in $ξ$ is replaced by consecutive integer numbers between $α$ and $β$ inclusive in ascending order. That produces a list of $|β −α|+ 1$ graphs, which are then connected according the specification of the corresponding range-enabled rule. The $α$ and $β$ themselves might refer to variables that are bound in the outer range-enabled rule.

In a well-formed graph:

each variable non-terminal (a letter from A to $Z)$ occurs at most once as $ν$ in $range(ν, α, β)$ rules;

all other occurrences of variable non-terminal that are allowed by the grammar are bound.

Note, that if a character sequence $ξ$ is a graph, then $ξ, c(ξ),$ c(1 , $ξ), t(ξ),$ and t(1 , $ξ)$ all denote the same graph. On the other hand, neither $loo_p(ξ)$ nor loop(1 , $ξ)$ are allowed.

The following examples illustrate these basic rules. The graphs have their first and last vertices marked with letters $F$ and $L$ correspondingly.

![](/upload/images2/cactus1.png)

![](/upload/images2/cactus2.png)



## 输入格式


The input file contains a single line with a well-formed cactus definition in SCGL. While the syntax and semantics of SCGL themselves do not guarantee that the resulting graph is a cactus, the input file for this problem always defines a cactus -- every edge belongs to at most one simple cycle and there are no multiple edges between vertices. For example, neither loop(3 , $loo_p(3))$ nor $loo_p(2)$ are possible.

The line in the input file is at most $1000$ characters long and defines a cactus with at most $50 000$ vertices. Integer numbers represented by number non-terminals do not exceed $50 000$ .



## 输出格式


The first line of the output file must contain two integer numbers $n$ and $m$ . Here $n$ is the number of vertices in the graph. Vertices are numbered from $1$ to $n$ , where $1$ is the number of the first vertex of the graph and $n$ is the number of the last vertex of the graph. The other vertices can be numbered arbitrarily. Edges of the graph are represented by a set of edge-distinct paths, where $m$ is the minimal number of such paths.

Each of the following $m$ lines must contain a path in the graph. A path starts with an integer number $k_{i} (k_{i} \ge 2)$ followed by $k_{i}$ integers from $1$ to $n$ . These $k_{i}$ integers represent vertices of a path. A path can go to the same vertex multiple times, but every edge must be traversed exactly once in the whole output file.



## 题目大意
### 题目描述

NEERC 以大量关于仙人掌的题目为特色——每条边属于至多一个简单环连通的无向图。直观的说，仙人掌是一种一些环被允许的广义树。

2005年，第一个有关仙人掌的问题出现，这个问题被简单的叫做[“仙人掌”](https://codeforces.com/gym/101334)。在2007年是[“仙人掌再来”](https://codeforces.com/gym/100273)，在2010年叫做[“仙人掌变革”](https://codeforces.com/gym/101309)，以及2013年是[“仙人掌自同构”](https://codeforces.com/gym/100307)。以下是这些问题中使用的仙人掌例子：

![](/upload/images2/cactus.png)

四年来评测必须为顶点以千数的仙人掌生成测试文件。当然，复杂性日益增加的大量数据发生器被建立，最终有一个被称为 CGL（Cactus Generator Language，仙人掌发生器语言）的领域特定语言。CGL 可以为测试的目的简洁地定义一个大仙人掌。本题中你要解析该语言的我们称为 SCGL（Simple Cactus Generator Language，简单仙人掌发生器语言）的一个简化版本，输出一个仙人掌作结果。

一个仙人掌要以列出边的极小集（覆盖全图的不同路径）输出。

SCGL 仙人掌定义的语法由语法中的指定的用下面的扩展巴科斯-诺尔范式的非终止图表示：

$$
\begin{aligned}
graph &= “\texttt{\textup{c}}”&&&&&&&&&&&&&&&&&&&&&&&&&&&\\
&| “\texttt{\textup{c(}}” list “\texttt{\textup{)}}”\\
&| “\texttt{\textup{loop(}}” list “\texttt{\textup{)}}”\\
&| “\texttt{\textup{t(}}” list “\texttt{\textup{)}}”\\
\end{aligned}
$$

$$
\begin{aligned}
list &= graph \{ “\texttt{\textup{,}}” graph \}&&&&&&&&&&&&\\
&|(number | range | variable ) [ “\texttt{\textup{,}}” graph ]\\
\end{aligned}
$$

$$
\begin{aligned}
&number = nzdig \{ “\texttt{\textup{0}}” | nzdig \}\\
&nzdig = “\texttt{\textup{1}}” | “\texttt{\textup{2}}” | \cdots | “\texttt{\textup{8}}” | “\texttt{\textup{9}}”\\
&range = “\texttt{\textup{range(}}” variable “\texttt{\textup{,}}” numvar “\texttt{\textup{,}}” numvar “\texttt{\textup{)}}”\\
&variable = “\texttt{\textup{A}}” | “\texttt{\textup{B}}” | \cdots | “\texttt{\textup{Y}}” | “\texttt{\textup{Z}}”\\
&numvar = number | variable
\end{aligned}
$$

一个图的制造规则表示一个有两个点标记的图——首和尾。图定义规则有以下语义：

- 基本建立块 $c$ 列表示一个仅有两个点（一首一尾）标记与一边的图。

- $c(σ)$ 规则对于含有 $n$ 个图的指定图列表 $σ$ 将第 $i$ 图尾顶点与第 $i+1$ 图首顶点合并，加入列表。（$i\in\mathbb{N}^*,1\le i< n$）结果图的首顶点为第一图首顶点，尾顶点为第 $n$ 图尾顶点。

- $loop(σ)$ 规则与 $c(σ)$相似，但第 $n$ 图尾顶点与第一图首顶点合并,加入列表。结果图的首尾顶点为列表中第一图首尾顶点。环仅可被应用于一图以上的列表。

- $t(σ)$ 规则连接一个指定图列表 $σ$，合并他们的首顶点。结果图的首尾顶点为列表中第一图首尾顶点。

图列表不是以一逗号分隔列表明确指定，就是用一个有一个数字、范围或变量的选择性地跟随一个逗号或图的可重列表指定。当一图非于一可重列表中明确指定，则该指定图被假定为 $c$。

最简单的可重列表用一个非终止数定义。它表示一个有指定整数个指定图的副本的列表。

一个可重范围列表由有三个组件（变量 $ν$，数字 $α$ 与 $β$）的 $range(ν, α, β)$ 规则定义。若 $ξ$ 字符序列为一图，则 $c|loop|t(range(ν, α, β), ξ)$ 被称为范围启用规则，变量 $ν$ 被称为 $ξ$ 中的一个约束变量。在一个范围启用规则的语境中，$ξ$ 被重复 $|β − α| + 1$ 次以建立列表。变量 $ν$ 于 $ξ$ 中的每次出现按升序由连续的 $α$ 与 $β$ 之间的整数（包括 $α$ 与 $β$）取代。 那产出一个包括 $|β −α|+ 1$ 个图的列表，通过相应的范围启用规则的规范连接。$α$ 与 $β$ 自身可能指被约束于外范围启用规则的变量。

在一个语法正确的图中：

- 每一个非终止变量（一个从 A 到 Z 的字母）作为 $range(ν, α, β)$ 规则中的 $ν$ 至多存在一次；

- 非终止变量的语法允许的所有其他事件被绑定。

注意，若一字符序列 $ξ$ 为一图，那么 $ξ, c(ξ), c(1 , ξ), t(ξ),$ 与 $t(1 , ξ)$ 都指此一图。另一方面，不论 $loop(ξ)$ 还是 $loop(1 , ξ)$ 都不被允许。

下列例子说明这些基本规则。这些图有以 F 与 L 相应标记的始末点。

![](/upload/images2/cactus1.png)

![](/upload/images2/cactus2.png)

### 输入格式

输入文件包含一行，含有一个 SCGL 定义。定义格式正确，总描述一仙人掌，每条边属于至多一个简单环，无重边。比如，$loop(3 , loop(3))$ 与 $loop(2)$ 都不可能。

输入文件中该行至多长 $1000$ 字符，定义的仙人掌至多 $50000$ 个顶点。由非终止数代列表的整数不超过 $50000$。
### 输出格式

输出文件第一行必须包含两个整数 $n$ 与 $m$。$n$ 为图顶点数。顶点由 $1$ 到 $n$ 编号，$1$ 为首点编号，$n$ 为图尾点编号。其他点可随意编号。图中边由一个边不重路径集代表，$m$为该集合最小路径数。

后 $m$ 行，每行必须包含图中一条路径。一条路径以一个整数 $k_{i} (k_{i} \ge 2)$ 开始，后随 $k_{i}$ 个整数从 $1$ 到 $n$。这 $k_{i}$ 个整数代列表一条路径的顶点。一条路径可经过同一顶点多次，但每条边必须在整个输出文件中刚好经过一次。

### 注释
此题中出现的的EBNF：

非终端符号为被定义的语言的句法部分。

终端符号为由一个或多个字符组成的序列，是构成语言的不可约元素。

本题中一条语法规则形如$元标识符=定义列表$

定义列表形如$主要句法|主要句法|\cdots$。

其中主要句法为可选序列、重复序列、分组序列、元标识符、终端字符串、空序列之一。

可选序列形如[定义列表]，重复序列形如{定义列表}，分组序列形如(定义列表)。

元标识符是以字母开头的字母数字序列，即非终端符号的名称。

由语法定义的语言的终端符号由终端字符串表示，终端字符串形如“一个或多个除该引号符号以外的任何终端字符的序列” 。

EBNF的终端符号称为终端字符，是字母、数字, 与`=|{}“()[]`字符之一。

需要注意的是，这里给出的EBNF不完整，但足以解决题目。

```input1
c(c,t(loop(3),c(c,loop(6))),loop(c,c,t(c,loop(4))))

```

```output1
15 1
19 1 2 9 10 11 12 13 10 15 9 14 2 3 4 5 6 7 8 3

```

```input2
c

```

```output2
2 1
2 1 2

```

```input3
c(2)

```

```output3
3 1
3 1 2 3

```

```input4
c(3)

```

```output4
4 1
4 1 2 3 4

```

```input5
t(c(3),c,c)

```

```output5
6 2
2 1 2
5 3 1 4 5 6

```

```input6
c(2,t(c(2),c,c))

```

```output6
9 3
3 2 1 3
3 4 5 6
5 1 7 5 8 9

```

## 提示
Time limit: 1 s, Memory limit: 256 MB. 



