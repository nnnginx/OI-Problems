## 题目描述


Jane is a game designer and she designs the next version of Jenga Boom, where the blocks have dimensions of $1 \times w \times w_n$ instead of the ordinary $1 \times 2 \times 6$ . As usual, the initial tower is created at the game start. It consists of the blocks in levels of $n$ blocks placed next to each other along their long sides and at a right angle to the previous level. Players remove blocks from the tower in turns, until the tower collapses.

![](https://onlinejudgeimages.s3.amazonaws.com/problem/13998/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202016-12-22%20%EC%98%A4%ED%9B%84%208.10.49.png)

Initial tower

![](https://onlinejudgeimages.s3.amazonaws.com/problem/13998/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202016-12-22%20%EC%98%A4%ED%9B%84%208.11.00.png)

The tower before collapse

Jane wants to build a game simulator that helps her to decide the best $n$ and $w$ . The simulator shall compute the moment when the tower collapses if blocks are removed in the specified order. Tower collapses if there is a cross-section between levels such that the center of the mass of the levels above it does not belong to or is at the edge of the convex hull of the previous level projection.



## 输入格式


The first line contains two integers $n$ and $w$ that define the dimensions of the block as described in the problem statement $(1 \le n , w \le 10 000)$ . The second line also contains two integers: $h$ -- the number of levels in the tower and $m$ -- the number of removed blocks $(1 \le h , m \le 5 000)$ .

The next $m$ lines contain coordinates of the removed blocks with two integers each: $l_{i}$ -- the level of the block, counting from the bottom and $k_{i}$ -- the position of the block, counting from the edge nearest to the players $(1 \le l_{i} \le h$ ; $1 \le k_{i} \le n)$ . Blocks are removed one by one and no block is removed twice.



## 输出格式


In the first line output `yes` if the tower collapses, and `no` otherwise. In the former case, output the number of the block (starting from $1$) , that was removed just before the collapse, in the next line.



## 题目大意
设有一个塔，它的积木块是 $1\times w\times (w\times n)$ 的长方体，每层由 $n$ 个积木块，每两层交错摆放，共有 $h$ 层。有 $m$ 个抽积木的操作，对于第 $i$ 个操作给出从底往上数的第 $l_i$ 层和从左后方往右前方数的第 $k_i$ 块。某一层的左边或右边加上中间 (如果 $n$ 为偶数，那么忽略中间) 的积木块全被抽完，则塔倒塌。

#### 输入格式
第一行为 $n$ 和 $w$ ，($1\le n,w\le10000$) 。第二行为 $h$ 和 $m$  ,($1\le h,m\le5000$)。接下来的 $m$ 行为 $l_i$ 和 $k_i$ ($1\le l_i\le h;1\le k_i\le n$) 。一块积木只能移动一次。
#### 输出格式
如果塔能倒塌，则输出 "yes" 。否则输出 "no" 。对于第一种情况，在下一行输出倒塌前一步的编号 $i$ 。

```input1
5 2
6 6
4 1
4 2
4 5
5 3
4 3
1 1

```

```output1
yes
5

```

```input2
3 3
10 1
10 3

```

```output2
no

```

```input3
2 2
2 1
1 1

```

```output3
yes
1

```

## 提示
Time limit: 2 s, Memory limit: 512 MB. 



