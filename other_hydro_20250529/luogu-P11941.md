## 题目背景
译自 [Natjecanje timova studenata informatičara hrvatskih sveučilišta](https://hsin.hr/studenti2024/) K.

## 题目描述
给定 $26$ 个只含小写英文字母的字符串 $s_a,s_b,\ldots,s_{z}$。

对于任意一个只含小写英文字母的字符串 $t$，我们把 $t$ 中的每个字母 $x$ 替换成字符串 $s_x$，得到新的字符串 $t'$。

> 例子：当 $s_a=\texttt{ana}$，$s_b=\texttt{ban}$ 时，
> 
> $t=\texttt{\textcolor{green}{b}a\textcolor{green}{b}a}\implies t'=\texttt{\textcolor{green}{ban}ana\textcolor{green}{ban}ana}$。

如果**存在**两个不同的字符串 $p,q$，它们在替换后得到的字符串 $p',q'$ 相同，亦即 $p\neq q$ 且 $p'=q'$，那么我们就说这个替换规则是坏的，否则我们说这个替换规则是好的。

试判断给定的替换规则是不是好的。


## 输入格式
**本题单个测试点内含有多组测试数据。**

第一行，正整数 $T$，表示测试数据组数。

接下来描述 $T$ 组测试数据：每组测试数据 $26$ 行，每行一个字符串，分别为 $s_a,s_b,\cdots,s_z$。

## 输出格式
对于每组测试数据，输出一行：

如果替换规则是好的，输出 $\texttt{Krasan}$（=克罗地亚语「漂亮的」）；

否则输出 $\texttt{Ruzan}$（$\texttt{ružan}$=克罗地亚语「丑陋的」）。

```input1
1
brainrot
time
gospodin
malnar
je
w
rizzler
i
veliki
sigma
te
ima
ogroman
gyatt
a
skibidi
toilet
nije
jer
zivi
u
ohiou
pa
placa
fanum
tax
```

```output1
Krasan
```

```input2
1
dotdash
dashdotdotdot
dashdotdashdot
dashdotdot
dot
dotdotdashdot
dashdashdot
dotdotdotdot
dotdot
dotdashdashdash
dashdotdash
dotdashdotdot
dashdash
dashdot
dashdashdash
dotdashdashdot
dashdashdotdash
dotdashdot
dotdotdot
dash
dotdotdash
dotdotdotdash
dotdashdash
dashdotdotdash
dashdotdashdash
dashdashdotdot
```

```output2
Ruzan
```

## 提示
#### 样例解释

样例 $2$ 解释：$\texttt{a}$ 和 $\texttt{et}$ 是一个符合条件的例子。

#### 数据范围

- $1\le t\le 10^4$；
- 输入的字符串长度和不超过 $10^6$。


