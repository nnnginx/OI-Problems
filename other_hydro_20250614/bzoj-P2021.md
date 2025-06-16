## 题目描述

Farmer John wants to save some blocks of his cows'delicious Wisconsin cheese varieties in his cellar for the coming winter. He has room for one tower of cheese in his cellar, and that tower's height can be at most $t$. The cows have provided him with a virtually unlimited number of blocks of each kind of $n$ different types of cheese (conveniently numbered $1\ldots n$). He'd like to store (subject to the constraints of height) the most valuable set of blocks he possibly can. The cows will sell the rest to support the orphan calves association.

Each block of the $i$-th type of cheese has some value $v_i$ and some height $h_i$, which is always a multiple of $5$.

Cheese compresses. A block of cheese that has height greater than or equal to K is considered "large" and will crush any and all of the cheese blocks (even other large ones) located below it in the tower. A crushed block of cheese doesn't lose any value, but its height reduces to just $\frac{4}{5}$ of its old height. Because the height of a block of cheese is always a multiple of $5$, the height of a crushed block of cheese will always be an integer. A block of cheese is either crushed or not crushed; having multiple large blocks above it does not crush it more. Only tall blocks of cheese crush other blocks; aggregate height of a tower does not affect whether a block is crushed or not.

What is the total value of the best cheese tower FJ can construct? Consider, for example, a cheese tower whose maximum height can be 53 to be build from three types of cheese blocks. Large blocks are those that are greater than or equal to $25$. Below is a chart of the values and heights of the various cheese blocks he stacks:

```plain
Type    Value      Height
1       100        25
2       20         5
3       40         10
```

FJ constructs the following tower:

```plain
          Type  Height Value
   top -> [1]   25     100
          [2]   4      20   <- crushed by [1] above
          [3]   8      40   <- crushed by [1] above
          [3]   8      40   <- crushed by [1] above
bottom -> [3]   8      40   <- crushed by [1] above
```

The topmost cheese block is so large that the blocks below it are crushed. The total height is: $25+4+8+8+8=53$. The total height does not exceed $53$ and thus is 'legal'. The total value is: $100+20+40+40+40=240$. This is the best tower for this particular set of cheese blocks.

John 要建一个奶酪塔，高度最大为 $t$。他有 $n$ 块奶酪。第 $i$ 块高度为 $h_i$（一定是 $5$ 的倍数），价值为 $v_i$。一块高度 $\geq k$ 的奶酪被称为大奶酪，一个奶酪如果在它上方有大奶酪（多块只算一次），它的高度就会变成原来的 $\frac{4}{5}$。很显然 John 想让他的奶酪他价值和最大。求这个最大值。

## 输入格式

第一行分别是 $n, t, k$。

接下来 $n$ 行分别是 $v_i, h_i$。

## 输出格式

一行最大值。

```input1
3 53 25
100 25
20 5
40 10
``` 
```output1
240
```

## 数据规模与约定

对于 $100\%$ 的数据，$1  \leq  k  \leq  t  \leq  10^3$，$1  \leq  n  \leq  100$，$1  \leq  v_i  \leq  10^6$，$5  \leq  h_i  \leq  t$。

## 题目来源

Silver