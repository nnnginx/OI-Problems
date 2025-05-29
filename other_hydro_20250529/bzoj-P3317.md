## 题目描述

Archibald and Adalbert are inseparable friends and the most knights of the whole kingdom. Competitive as they are, they accasionally engage in a little open-air sword fight, just to determine who among them really is the first knight. Of course, neither Adalbert nor Archibald wins, but they keep themselves busy for quite a while and get around in the surroundings. You have to calculate about how long their next 'fight' will last.

All the action takes place in a rectangular area which, for the sake of simplicity, is divided into unit squares numbered from $(1,1)$ to $(m,n)$. Starting at $(1,1)$, the knights move from one square to one of the at most four adjacent squares, and finish as soon as they reach $(m,n)$ where the tavern is located.

At each square, it is largely a matter of chance where the fight will continue, but it also depends on the environment (for example, if a certain direction is uphill). Our model uses probabilities to decide into which adjacent square the fight will move next. (For example, an uphill direction has a lower probability.) It is your job to calculate the expected number of moves that are needed before the tavern is reached. You can assume that every move is independent of the directions chosen in the preious moves.

## 输入格式

The input consists of a sequence of rectangular areas. Each area starts with a line containing the dimensions of the rectangle $m$ and $n$. Four blocks follow that state the probability of a move in each direction. Every block contains $m$ lines, and each line contains $n$ numbers $p_{i,j}^{(k)}$. The porbabilities in block $k$ are arranged as follows:

$$ \begin{matrix}p_{1,1}^{(k)}&p_{1,2}^{(k)}&p_{1,3}^{(k)}&\cdots&p_{1,n-1}^{(k)}&p_{1,n}^{(k)}\\p_{2,1}^{(k)}&p_{2,2}^{(k)}&p_{2,3}^{(k)}&\cdots&p_{2,n-1}^{(k)}&p_{2,n}^{(k)}\\\vdots\\p_{m,1}^{(k)}&p_{m,2}^{(k)}&p_{m,3}^{(k)}&\cdots&p_{m,n-1}^{(k)}&p_{m,n}^{(k)}\end{matrix}$$

The number $p_{i,j}^{(k)}$ gives the probability of a move from square $(i,j)$ to the next square: In block $1$ this is $(i+1,j)$, in block $2$ it is $(i,j+1)$, in block $3$ it is $(i-1,j)$ and in block $4$ it is $(i,j-1)$. For each square $(i,j)$ except the tavern $(m,n)$, the porbabilities $p_{i,j}^{(k)}$ add uo to $1$ and at least one of $p_{i,j}^{(1)}$ or $p_{i,j}^{(2)}$ is not $0$. (This ensures that the tavern will finally be reached with probability $1$.) You may assume that the probability of moving outside the rectagle is $0$, as are $p_{m,n}^{(k)}$ for all $k$. The sequence of areas is followed by a line containing two zeros.

## 输出格式

For each area, output a line containing the expected number of moves from $(1,1)$ to $(m,n)$. This number must have an absolute error less than $0.1$ compared.

## 中文简述

一个 $m\times n$ 的棋盘，左上至右下编号为 $(1,1)$ 至 $(m,n)$，并给定每个格子到周围四个格子的概率。

一个骑士从 $(1,1)$ 开始，按照给定概率走，问到达 $(m,n)$ 的期望步数。 

题目保证从任一格开始到 $(m,n)$ 的概率均为 $1$。

```input1
2 2
0.01 0.50
0.00 0.00
0.99 0.00
0.50 0.00
0.00 0.00
0.50 0.00
0.00 0.50
0.00 0.00
1 5
0.0 0.0 0.0 0.0 0.0
1.0 0.1 0.7 0.5 0.0
0.0 0.0 0.0 0.0 0.0
0.0 0.9 0.3 0.5 0.0
3 3
0.000001 0.0 1.0
0.0 1.0 1.0
0.0 0.0 0.0
0.999999 1.0 0.0
1.0 0.0 0.0
0.000001 0.000001 0.0
0.0 0.0 0.0
0.0 0.0 0.0
0.999999 0.0 0.0
0.0 0.0 0.0
0.0 0.0 0.0
0.0 0.999999 0.0
0 0
```

```output1
4.0
41.142857142857146
7.999994000002
```

## 数据规模与约定

For $100\%$ data, $1\leq m,n\leq 40$, $0\leq p_{i,j}^{(k)}\leq 1$, answer that is always less than $10^6$.

## 题目来源

WCMG 提供 SPJ。