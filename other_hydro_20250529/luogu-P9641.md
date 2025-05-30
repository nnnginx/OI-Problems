## 题目描述
BaoBao has just found a grid with $n$ rows and $m$ columns in his left pocket, where the cell in the $j$-th column of the $i$-th row (indicated by $(i, j)$) contains an arrow (pointing either upwards, downwards, leftwards or rightwards) and an integer $a_{i, j}$.

BaoBao decides to play a game with the grid. He will first select a cell as the initial cell and tick it. After ticking a cell (let's say BaoBao has just ticked cell $(i, j)$), BaoBao will go on ticking another cell according to the arrow and the integer in cell $(i, j)$.

- If the arrow in cell $(i, j)$ points upwards, BaoBao will go on ticking cell $(i-a_{i, j}, j)$ if it exists.
- If the arrow in cell $(i, j)$ points downwards, BaoBao will go on ticking cell $(i+a_{i, j}, j)$ if it exists.
- If the arrow in cell $(i, j)$ points leftwards, BaoBao will go on ticking cell $(i, j-a_{i, j})$ if it exists.
- If the arrow in cell $(i, j)$ points rightwards, BaoBao will go on ticking cell $(i, j+a_{i, j})$ if it exists.

If the cell BaoBao decides to tick does not exist, or if the cell is already ticked, the game ends.

BaoBao is wondering if he can select a proper initial cell, so that he can tick every cell in the grid exactly once before the game ends. Please help him find the answer.


## 输入格式
There are multiple test cases. The first line contains an integer $T$, indicating the number of test cases. For each test case:

The first line contains two integers $n$ and $m$ ($1 \le n \times m \le 10^5$), indicating the number of rows and columns of the grid.

For the following $n$ lines, the $i$-th line contains a string $s_i$ consisting of lowercased English letters ($|s_i| = m$, $s_{i, j} \in \{\text{`u' (ascii: 117)}, \text{`d' (ascii: 100)}, \text{`l' (ascii: 108)}, \text{`r'(ascii: 114)}\}$), where $s_{i, j}$ indicates the direction of arrow in cell $(i, j)$.

- If $s_{i, j} = \text{`u'}$, the arrow in cell $(i, j)$ points upwards.
- If $s_{i, j} = \text{`d'}$, the arrow in cell $(i, j)$ points downwards.
- If $s_{i, j} = \text{`l'}$, the arrow in cell $(i, j)$ points leftwards.
- If $s_{i, j} = \text{`r'}$, the arrow in cell $(i, j)$ points rightwards.

For the following $n$ lines, the $i$-th line contains $m$ integers $a_{i, 1}, a_{i, 2}, \dots, a_{i, m}$ ($1 \le a_{i, j} \le \max(n, m)$), where $a_{i, j}$ indicates the integer in cell $(i, j)$.

It's guaranteed that the sum of $n \times m$ of all test cases does not exceed $10^6$.

## 输出格式
For each test case output one line. If BaoBao can find a proper initial cell, print ``Yes`` (without quotes), otherwise print ``No`` (without quotes).


## 题目大意
**【题目描述】**

宝宝刚刚在他的左口袋里发现了一个 $n$ 行 $m$ 列的网格，其中第 $i$ 行第 $j$ 列的单元格（表示为 $(i, j)$）包含一个箭头（指向上、下、左或右）和一个整数 $a_{i, j}$。

宝宝决定用这个网格玩一个游戏。他首先会选择一个单元格作为初始单元格并标记它。在标记一个单元格之后（假设宝宝刚刚标记了单元格 $(i, j)$），宝宝将根据单元格 $(i, j)$ 中的箭头和整数继续标记另一个单元格。

- 如果单元格 $(i, j)$ 中的箭头指向上方，宝宝将继续标记单元格 $(i-a_{i, j}, j)$，如果该单元格存在的话。
- 如果单元格 $(i, j)$ 中的箭头指向下方，宝宝将继续标记单元格 $(i+a_{i, j}, j)$，如果该单元格存在的话。
- 如果单元格 $(i, j)$ 中的箭头指向左方，宝宝将继续标记单元格 $(i, j-a_{i, j})$，如果该单元格存在的话。
- 如果单元格 $(i, j)$ 中的箭头指向右方，宝宝将继续标记单元格 $(i, j+a_{i, j})$，如果该单元格存在的话。
如果宝宝决定标记的单元格不存在，或者该单元格已经被标记，游戏结束。

宝宝想知道他是否可以选择一个合适的初始单元格，以便在游戏结束前恰好标记网格中的每一个单元格一次。请帮助他找到答案。

**【输入格式】**

有多个测试用例。第一行包含一个整数 $T$，表示测试用例的数量。对于每个测试用例：

第一行包含两个整数 $n$ 和 $m$ ($1 \le n \times m \le 10^5$)，表示网格的行数和列数。

接下来的 $n$ 行中，第 $i$ 行包含一个字符串 $s_i$，由小写英文字母组成（$|s_i| = m$，$s_{i, j} \in \{\text{`u' (ascii: 117)}, \text{`d' (ascii: 100)}, \text{`l' (ascii: 108)}, \text{`r'(ascii: 114)}\}$），其中 $s_{i, j}$ 表示单元格 $(i, j)$ 中箭头的方向。

- 如果 $s_{i, j} = \text{`u'}$，单元格 $(i, j)$ 中的箭头指向上方。
- 如果 $s_{i, j} = \text{`d'}$，单元格 $(i, j)$ 中的箭头指向下方。
- 如果 $s_{i, j} = \text{`l'}$，单元格 $(i, j)$ 中的箭头指向左方。
- 如果 $s_{i, j} = \text{`r'}$，单元格 $(i, j)$ 中的箭头指向右方。

接下来的 $n$ 行中，第 $i$ 行包含 $m$ 个整数 $a_{i, 1}, a_{i, 2}, \dots, a_{i, m}$ ($1 \le a_{i, j} \le \max(n, m)$)，其中 $a_{i, j}$ 表示单元格 $(i, j)$ 中的整数。

保证所有测试用例的 $n \times m$ 之和不超过 $10^6$。

**【输出格式】**

对于每个测试用例输出一行。如果宝宝可以找到一个合适的初始单元格，输出 “Yes”（不含引号），否则输出 “No”（不含引号）。

**【样例解释】**

对于第一个示例测试用例，宝宝可以选择单元格 $(1, 2)$ 作为初始单元格，这样他可以按以下顺序恰好打勾所有单元格：$(1, 2), (2, 2), (2, 3), (2, 1), (1, 1), (1, 3)$。

对于第二个示例测试用例，无论选择哪个单元格作为初始单元格，宝宝最多只能打勾 2 个单元格。

翻译来自于：[ChatGPT](https://chatgpt.com/)。

```input1
2
2 3
rdd
url
2 1 1
1 1 2
2 2
rr
rr
1 1
1 1
```

```output1
Yes
No
```

## 提示
For the first sample test case, BaoBao can select cell $(1, 2)$ as the initial cell, so that he can tick all the cells exactly once in the following order: $(1, 2), (2, 2), (2, 3), (2, 1), (1, 1), (1, 3)$.

For the second sample test case, BaoBao can only tick at most $2$ cells no matter which cell is selected as the initial cell.


