## 题目描述
Prof. Pang built $n$ block towers with different heights. The $i$-th tower has height $a_i$.

Prof. Shou doesn't like these towers because of their arbitrary heights. He decides to $\textbf{first remove exactly \textit{m} of them}$, and then perform some (or none) of the following operations: 

- Choose a tower and increase its height $a_i$ by $1$. 
- Choose a tower and decrease its height $a_i$ by $1$.
- Choose a tower and divide its height $a_i$ by $2$. If the new height is not an integer, it is rounded down. 

Prof. Shou can never choose a removed tower. If after an operation, the height of a tower will become $0$, that operation is not allowed. Under these constraints, Prof. Shou can perform an arbitrary number of operations in arbitrary order. 

Prof. Shou would like all the towers that are not removed to have the same heights. Please calculate the minimum number of operations to achieve this.

## 输入格式
The first line contains one integer $T~(1\le T \le 10)$, the number of test cases.

For each test case, the first line contains two integers $n, m~(1\le n\le 500, 0\le m <n)$, the number of towers, and the number of towers Prof. Shou should delete before performing the operations.

The next line contains $n$ integers $a_1,\ldots, a_n~(1\le a_i\le 10^9)$, the initial heights of the towers.

## 输出格式
For each test case, output the minimum number of operations in one line.

## 题目大意
### 题目描述
庞教授搭了 $n$ 座不同高度的塔。第 $i$ 座塔的高度是 $a _ {i}$。

寿教授不喜欢这些参差不齐的塔。他决定**先去掉它们中的 $m$ 座**，然后执行以下操作中的一些（或不执行）：
- 选择一座塔并增加它 $1$ 个单位高度。
- 选择一座塔并减少它 $1$ 个单位高度。
- 选择一座塔并把它的高度 $a _ {i}$ 除以 $2$，如果它不是整数的话，向下取整。

寿教授永远不会选择被拆除的塔。如果操作后，塔的高度变为 $0$，则不允许操作。在这些约束条件下，寿教授可以按任意顺序执行任意数量的运算。

寿教授希望所有没有被拆除的塔都有相同的高度 $a _ {i}$。请计算实现此目标的最小操作次数。
### 输入格式
第一行是一个整数 $T(1\leqslant$ $T$ $\leqslant$ $10)$,表示有 $T$ 组数据。

对于每组测试数据，第一行包括两个整数 $n,m (1\leqslant$ $n$ $\leqslant$ $500$$,$$0$ $\leqslant$ $m$ $\leqslant$ $n$$)$，表示塔的数量以及寿教授在执行操作之前应该删除的塔的数量。

下一行包括 $n$ 个整数 $a _ {1},\dots,a _ {n} (1\leqslant$ $a _ {i}$ $\leqslant$ $10^9)$，表示塔的最初高度。
### 输出格式
对于每组测试数据，在一行中输出最小操作数。

```input1
3
2 0
2 6
5 0
1 2 3 4 5
5 3
1 2 3 4 5
```

```output1
2
4
1
```

