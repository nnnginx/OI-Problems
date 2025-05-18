## 题目描述
Farmer John is continuing to ponder the issue of cows crossing the road through his farm, introduced in the preceding two problems. He realizes now that the threshold for friendliness is a bit more subtle than he previously considered -- breeds $a$ and $b$ are now friendly if $|a - b| \leq K$, and unfriendly otherwise.
Given the orderings of fields on either side of the road through FJ's farm, please count the number of unfriendly crossing pairs of breeds, where a crossing pair of breeds is defined as in the preceding problems.



## 输入格式
The first line of input contains $N$ ($1 \leq N \leq 100,000$) and $K$ ($0 \leq K < N$). The next $N$ lines describe the order, by breed ID, of fields on one side of the road; each breed ID is an integer in the range $1 \ldots N$. The last $N$ lines describe the order, by breed ID, of the fields on the other side of the road. Each breed ID appears exactly once in each ordering.


## 输出格式
Please output the number of unfriendly crossing pairs of breeds.



## 题目大意
### 题目描述

Farmer John 继续思考奶牛穿过他农场道路的问题，这个问题在前两个问题中已经介绍过。他现在意识到，友好度的阈值比他之前考虑的要微妙一些——现在，品种 $a$ 和 $b$ 是友好的当且仅当 $|a - b| \leq K$，否则就是不友好的。给定 FJ 农场道路两侧田地的品种顺序，请计算不友好的交叉品种对的数量，其中交叉品种对的定义与前两个问题相同。

### 输入格式

输入的第一行包含 $N$ ($1 \leq N \leq 100,000$) 和 $K$ ($0 \leq K < N$)。接下来的 $N$ 行描述了道路一侧田地的品种顺序；每个品种 ID 是一个在 $1 \ldots N$ 范围内的整数。最后的 $N$ 行描述了道路另一侧田地的品种顺序。每个品种 ID 在每个顺序中恰好出现一次。

### 输出格式

请输出不友好的交叉品种对的数量。

### 说明/提示

在这个例子中，品种 1 和 4 是不友好的且交叉的，品种 1 和 3 也是不友好的且交叉的。

```input1
4 1
4
3
2
1
1
4
2
3
```

```output1
2
```

## 提示
In this example, breeds 1 and 4 are unfriendly and crossing, as are breeds 1 and 3.



