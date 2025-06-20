# AT_agc068_e [AGC068E] Sort and Match

## 题目描述

给定一个大小为 $N \times N$ 的整数矩阵 $A = (A_{i,j})_{1 \leq i, j \leq N}$ 和一个整数 $M$。

对于长度为 $M$ 的整数序列 $x = (x_1, x_2, \cdots, x_M)$，其中每个元素均为 $1$ 到 $N$ 之间的整数，我们定义一个函数 $f(x)$：

- 首先将序列 $x$ 中的元素按照非严格递增顺序排列，得到新序列 $y = (y_1, y_2, \cdots, y_M)$。
- 计算 $f(x) = \prod_{1 \leq i \leq M} A_{x_i, y_i}$。

请对每一个 $k = 1, 2, \cdots, N$ 计算以下问题：

- 对所有满足 $x_1 = k$ 的序列 $x$，计算它们对应的 $f(x)$ 的总和，并将结果对 $998244353$ 取模。

## 输入格式

输入包含以下内容，从标准输入读取：

> 第一行为两个整数，$N$ 和 $M$。  
> 接下来为一个 $N \times N$ 的矩阵，按行优先顺序给出：  
> $A_{1,1}$ $A_{1,2}$ $\cdots$ $A_{1,N}$  
> $A_{2,1}$ $A_{2,2}$ $\cdots$ $A_{2,N}$  
> $\vdots$  
> $A_{N,1}$ $A_{N,2}$ $\cdots$ $A_{N,N}$

## 输出格式

按顺序输出每个 $k = 1, 2, \cdots, N$ 的答案。

## 输入输出样例 #1

### 输入 #1

```
2 2
1 2
3 4
```

### 输出 #1

```
5 22
```

## 输入输出样例 #2

### 输入 #2

```
2 3
1 2
3 4
```

### 输出 #2

```
27 118
```

## 输入输出样例 #3

### 输入 #3

```
5 4
785439575 250040585 709423541 945005786 19237225
404191279 250876592 22672563 519729086 344065186
273714212 560047125 139793596 542901248 520999410
855572558 498896932 418633758 742973826 248730678
238856535 319502970 908902333 164543594 245101681
```

### 输出 #3

```
216530400 726773157 717209375 797938347 957133905
```

## 输入输出样例 #4

### 输入 #4

```
10 50
197971506 714635866 966125570 768080799 80565655 459117401 256810168 775681305 582857561 948631706
437330820 321722967 531470304 255908811 45459908 504089816 695016247 91058795 905527130 30860430
151769562 979797105 619322493 298241991 360690308 480124392 297323928 284686636 922571073 627798362
753705854 712639027 721488863 69714419 485979799 88704853 758288417 423073188 595934547 86264514
272481811 622712481 221745114 225051881 433378197 985573661 210619166 851716760 283615535 834897126
366075547 933505674 858395194 490049033 22039836 361481447 735151983 518458804 422209788 28981946
907645400 111982636 978445563 686621115 486475154 734616351 587635888 527524079 454844580 826849288
868863954 490627044 967828344 887235558 138021910 435784230 343307056 118718683 547282350 757693154
32344652 101428952 585897722 693817619 790433406 848494439 873744405 604427602 951889915 989125209
865548541 642980476 603592935 911086893 466178404 79002814 902745597 825893950 147052664 805753279
```

### 输出 #4

```
862518623 606960987 762676180 606184511 762408948 47716007 968649097 788324707 140177479 484063588
```

## 说明/提示

### 约束条件

- $1 \leq N \leq 50$
- $1 \leq M \leq 50$
- $0 \leq A_{i,j} < 998244353$
- 所有输入数据都是整数

### 示例说明

对于所有可能的序列 $x$ 及其 $f(x)$ 值如下：
- 对于 $x = (1, 1)$，产生排序后序列 $y = (1, 1)$，因此 $f(x) = A_{1,1} \times A_{1,1} = 1$。
- 对于 $x = (1, 2)$，产生排序后序列 $y = (1, 2)$，因此 $f(x) = A_{1,1} \times A_{2,2} = 4$。
- 对于 $x = (2, 1)$，产生排序后序列 $y = (1, 2)$，因此 $f(x) = A_{2,1} \times A_{1,2} = 6$。
- 对于 $x = (2, 2)$，产生排序后序列 $y = (2, 2)$，因此 $f(x) = A_{2,2} \times A_{2,2} = 16$。

所以，当 $k = 1$ 时，答案是 $1 + 4 = 5$，当 $k = 2$ 时，答案是 $6 + 16 = 22$。

 **本翻译由 AI 自动生成**