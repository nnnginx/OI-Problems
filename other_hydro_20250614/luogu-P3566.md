## 题目描述
Little Bitie and his friends spent the whole yesterday playing    with colorful bricks in the kindergarten.

Initially they made building models but they quickly got bored with that.

Then they decided to place the bricks in a line, one after another.

To avoid a dull look, they tried to avoid putting two bricks of the same    color next to each other.

After a long while they succeeded in placing all the bricks while observing    this rule.

Then the day care was over, and the children went home with their parents.

Today Bitie came to the kindergarten early.

He was satisfied to see that their yesterday's creation was still standing.

But then he tripped over in a most unfortunate way,    falling right on the line of bricks, which all mixed in a pile.

The boy quickly sorted them by color and wondered how best to quickly    reassemble the perfect line.

He managed to recall what were the colors of the two bricks on both end of the line.

Help little Bitie out and tell him how to order the bricks in a line so that    no two bricks of the same color are next to each other and the bricks at the ends    of the line have the colors that he recalled.

Note that Bitie could have made a mistake in recalling the two colors    or perhaps he did not find some of the blocks after falling into them,    so the reconstruction might not be possible.

## 输入格式
There are three integers in the first line of the standard input,    $k$,$p$, and $q$ ($1\le k\le 1 000 000$,$1\le p,q\le k$), separated by single spaces,    denoting the number of brick colors, and the colors of    the first and the last brick in the desired arrangement, respectively.

In the second line, there are $k$ integers,$i_{1},i_{2},...,i{k}$ ($1\le i_{j}\le 1 000 000$),    separated by single spaces.

The number $i_{j}$ signifies that Bitie has exactly $i_{j}$ bricks    of color $j$.

You may assume that the total number of bricks does not exceed one million, i.e., that $n=i_1+i_2+\cdots+i_k\le 1\ 000\ 000$.


## 输出格式
Your program should print $n$ integers to the standard output,    separated by single spaces.

The numbers should represent the colors of successive bricks in    an arrangement that satisfies aforementioned constraints.

If no such arrangement exists, your program should print only    a single integer: $0$.

If there are several correct answers, your program can pick one    arbitrarily.


## 题目大意
### 题目描述

现在你有 $k$ 种颜色的砖块，已知每种颜色砖块的数量，问是否有一种方案可以将砖块放成一排并且第一块和最后一块砖块的颜色为 $p,q$ 且相邻的砖块颜色不同，如果没有合法方案则输出 $0$。

### 输入格式

第一行输入三个整数 $k,p,q$ 分别代表砖块有 $k$ 种颜色，第一块和最后一块的砖块颜色分别是 $p,q$，第二行输入 $k$ 个数，第 $j$ 个数表示颜色为 $j$ 砖块的数量。

### 输出格式

输出一个排列，要求用完全部砖块并且满足上述约束条件，如果有多个正确答案只需要输出其中一种，特别的，如果无解输出 $0$。在最后一个数字后请不要输出空格。

### 数据范围

$1 \leq k \leq 1e6,1\leq p,q \leq k$。

其中保证砖块总数量之和不超过 $1e6$。

```input1
3 3 1
2 3 3

```

```output1
3 2 1 3 2 3 2 1

```

