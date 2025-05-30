## 题目背景
### Warning: If you submit a malicious program, you will be banned.
### 警告：恶意提交本题将被封号。


## 题目描述
Ceramic artists Maria and João are opening a small azulejo store in Porto. Azulejos are the beautiful ceramic tiles for which Portugal is famous. Maria and João want to create an attractive window display, but, due to limited space in their shop, they must arrange their tile samples in two rows on a single shelf. Each of João's tiles has exactly one of Maria's tiles in front of it and each of Maria's tiles has exactly one of João's tiles behind it. These hand-crafted tiles are of many different sizes, and it is important that each tile in the back row is taller than the tile in front of it so that both are visible to passers-by. For the convenience of shoppers, tiles in each row are arranged in non-decreasing order of price from left to right. Tiles of the same price may be arranged in any order subject to the visibility condition stated above.

Your task is to find an ordering of the tiles in each row that satisfies these constraints, or determine that no such ordering exists.

## 输入格式
The first line of input contains an integer $n$ ($1 \leq n \leq 5 \times 10^5$), the number of tiles in each row. The next four lines contain $n$ integers each; the first pair of lines represents the back row of tiles and the second pair of lines represents the front row. Tiles in each row are numbered from $1$ to $n$ according to their ordering in the input. The first line in each pair contains $n$ integers $p_1, \dots , p_n$ ($1 \leq p_i \leq 10^9$ for each $i$), where $p_i$ is the price of tile number $i$ in that row. The second line in each pair contains $n$ integers $h_1, \dots , h_n$ ($1 \leq h_i \leq 10^9$ for each $i$), where $h_i$ is the height of tile number $i$ in that row.

## 输出格式
If there is a valid ordering, output it as two lines of $n$ integers, each consisting of a permutation of the tile numbers from $1$ to $n$. The first line represents the ordering of the tiles in the back row and the second
represents the ordering of the tiles in the front row. If more than one pair of permutations satisfies the constraints, any such pair will be accepted. If no ordering exists, output `impossible`.

## 题目大意
给你两种瓷砖 $a,b$，每种瓷砖有 $n$ 块，每块瓷砖有两个属性：高度 $h$ 和价值 $p$。

现在要求你把这些瓷砖重新排成两行（$2\times n$）。前一行放瓷砖 $b$，后一行放瓷砖 $a$。

要求从左到右 $p$ 递增（单调不减），对于任意一个位置 $i$，后面的瓷砖要比前面的瓷砖高。

求一种方案或输出无解。

$n\le 5\times 10^5$

```input1
4
3 2 1 2
2 3 4 3
2 1 2 1
2 2 1 3
```

```output1
3 2 4 1
4 2 1 3
```

```input2
2
1 2
2 3
2 8
2 1
```

```output2
impossible
```

## 提示
Source: ICPC 2019 World Finals.

