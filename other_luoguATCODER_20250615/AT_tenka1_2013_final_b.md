# AT_tenka1_2013_final_b 天下一マジック

## 题目描述

高桥君是某公司的总裁，他想通过表演一场魔术来活跃员工的气氛。为了让这个魔术成功，他需要在不被发现的情况下，神速地将看似随意排列的卡片排序。

卡片的数量为 $2N+1$，这是一个奇数。为了方便，每张卡片上都标有编号，从 $1$ 到 $2N+1$。高桥君可以连续执行以下两种操作来重新排列卡片。集合 $X$ 包含了从 $1$ 到 $2N$ 的整数。

**操作 1（切牌）**：  
从集合 $X$ 中挑选一个数 $K$，将最前面的 $K$ 张卡片拿起，保持顺序不变地放在当前卡片的末尾。例如，如果 $K=3$，那么经过操作，卡片顺序将从 \[5, 1, 4, 7, 6, 2, 3\] 变为 \[7, 6, 2, 3, 5, 1, 4\]。

**操作 2（交替洗牌）**：  
将卡片前 $N+1$ 张和剩下的 $N$ 张分开，然后从每组中轮流依次取一张，组建新的一列，从 $N+1$ 张的那组开始。例如，卡片顺序从 \[5, 1, 4, 7, 6, 2, 3\] 变为 \[5, 6, 1, 2, 4, 3, 7\]。

给定卡片的初始顺序和集合 $X$，请计算出高桥君最少需要多少次操作才能将卡片按升序排列。如果无法实现这种排列，就输出 `-1`。

- 如果能解决 $1 \leq N \leq 4$ 且 $X = \{1\}$ 的情况，你将获得满分 $200$ 分中的 $20$ 分。
- 如果能解决 $1 \leq N \leq 2013$ 且 $X = \{1\}$ 的情况，可以额外获得 $80$ 分。
- 对于 $0 \leq N \leq 2013$ 且 $0 \leq M < 2N+1$ 的各类情况，剩余的 $100$ 分将被给予。

输出要求的最小操作次数。如果无法完成排序，输出 `-1`。记得在输出的最后留一个换行。

## 示例

输入：
```
1 1
3 2 1
1
```

输出：
```
2
```

输入：
```
2 1
3 2 5 1 4
1
```

输出：
```
-1
```

- 这种排列无法通过任何操作达到升序。

输入：
```
2 1
4 2 5 3 1
1
```

输出：
```
4
```

- 可以按以下步骤完成：
  - 施行操作 2：\[4, 2, 5, 3, 1\] → \[4, 3, 2, 1, 5\]
  - 再次操作 2：\[4, 3, 2, 1, 5\] → \[4, 1, 3, 5, 2\]
  - 施行操作 1，$K=1$：\[4, 1, 3, 5, 2\] → \[1, 3, 5, 2, 4\]
  - 再次操作 2：\[1, 3, 5, 2, 4\] → \[1, 2, 3, 4, 5\]

输入：
```
3 1
1 2 3 4 5 6 7
1
```

输出：
```
0
```

- 卡片最初就已经按升序排列，所需操作次数为 0。

输入：
```
4 2
2 3 4 5 6 7 8 9 1
1 6
```

输出：
```
3
```

- 通过以下步骤实现：
  - 操作 1，$K=1$：\[2, 3, 4, 5, 6, 7, 8, 9, 1\] → \[3, 4, 5, 6, 7, 8, 9, 1, 2\]
  - 操作 1，$K=6$：\[3, 4, 5, 6, 7, 8, 9, 1, 2\] → \[9, 1, 2, 3, 4, 5, 6, 7, 8\]
  - 操作 1，$K=1$：\[9, 1, 2, 3, 4, 5, 6, 7, 8\] → \[1, 2, 3, 4, 5, 6, 7, 8, 9\]

## 输入格式

第一行包含两个整数 $N$ 和 $M$，分别表示卡片数量的一半和集合 $X$ 的元素个数。
第二行是卡片的初始排列。
第三行给出集合 $X$ 中的元素。

## 输出格式

输出一个整数，表示将卡片排列为升序所需的最少操作次数。如果无法完成，输出 `-1`。

## 说明/提示

- $0 \leq N \leq 2013$
- $0 \leq M < 2N+1$

 **本翻译由 AI 自动生成**