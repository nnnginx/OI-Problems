## 题目描述
Chino 刚学习了一种叫做线段树的数据结构。可是她在写线段树时遇到了一个问题：她不知道该使用多大的空间，只知道线段树的叶子结点个数 $n$ 为一个在范围 $[a,b]$ 之内的正整数。

Chino 设 $f(n)$ 表示一棵 $n$ 个叶子结点的线段树所占的最大数组下标。她觉得如果她知道了

$$\sum_{n=a}^{b}f(n)$$

那么她就能够算出她需要多少使用多大的空间。所以她来请教聪明的你来帮帮她。

具体地，Chino 构建线段树的伪代码如下：

$$
\def\b#1{\textbf{#1}}\def\t#1{\text{#1}}\def\s\qquad\def\P{\mathbb P}\def\l{\underline{\kern{300pt}}}\def\m#1{#1&\,}
\def\if#1{\b{if }#1\b{ then}}\def\endfunc{\b{end function}.}\def\endif{\b{end if}.}\def\func{\b{function}}\def\return{\b{return}}
\begin{aligned}&\l\\&\b{Function: }\t{Build a Segment Tree.}\\[-10pt]&\l\\[-5pt]&\begin{array}{r|l}\\[-9pt]
\m1\func\ \t{BuildSegmentTree}\left(x,l,r\right):\\
\m2\s\if{\left(l\ne r\right)}:\\
\m3\s\s m\gets\left\lfloor\left(l+r\right)/2\right\rfloor.\\
\m4\s\s\t{BuildSegmentTree}\left(2x,l,m\right).\\
\m5\s\s\t{BuildSegmentTree}\left(2x+1,m+1,r\right).\\
\m6\s\endif\\
\m7\endfunc\\[-10pt]\\\end{array}\\[-13pt]&\l\end{aligned}
$$

线段树所占的最大数组下标即为在 $\def\t#1{\text{#1}}\t{BuildSegmentTree}\left(1,1,n\right)$ 后所有调用的 $\def\t#1{\text{#1}}\t{BuildSegmentTree}$ 中参数 $x$ 的最大值。

## 输入格式
输入共二行。

第一行为一个正整数 $a$；第二行为一个正整数 $b$。其意义如题面所述。

## 输出格式
输出一行一个正整数，表示你的答案。

```input1
1
10

```

```output1
108

```

```input2
233333
666666

```

```output2
588544964910

```

```input3
1
1000000000000000000

```

```output3
1419691012023749904603586777179575510

```

## 提示
### 样例解释 #1
$1\sim 10$ 个叶子结点的线段树的最大下标分别为 $1,3,5,7,9,13,13,15,17,25$，求和得到 $108$。

### 测试点约束
**本题采用捆绑测试。**

对于全部数据，有 $1\le a\le b\le10^{10^6}$。

每个子任务的具体限制见下表：

| 子任务编号 | 分值 | $b\le$ | $a=b$ |
|:-:|:-:|:-:|:-:|
| 1 | 10 | $10^{10^0}$ | $\times$ |
| 2 | 10 | $10^{10^1}$ | $\times$ |
| 3 | 10 | $10^{10^2}$ | $\times$ |
| 4 | 10 | $10^{10^3}$ | $\surd$ |
| 5 | 10 | $10^{10^3}$ | $\times$ |
| 6 | 10 | $10^{10^4}$ | $\surd$ |
| 7 | 10 | $10^{10^4}$ | $\times$ |
| 8 | 10 | $10^{10^5}$ | $\surd$ |
| 9 | 10 | $10^{10^5}$ | $\times$ |
| 10 | 10 | $10^{10^6}$ | $\times$ |

