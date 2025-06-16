## 题目描述
The cows are going to space! They plan to achieve orbit by building a sort of space elevator:  
a giant tower of blocks. They have $k \ (1 \le k \le 400)$ different types of blocks with which to build the tower. Each block of type $i$ has height $h_i \ (1 \le h_i \le 100)$ and is available in quantity $c_i \ (1 \le c_i \le 10)$. Due to possible damage caused by cosmic rays, no part of a block of type $i$ can exceed a maximum altitude $a_i \ (1 \le a_i \le 4\times 10^4)$. Help the cows build the tallest space elevator possible by stacking blocks on top of each other according to the rules.

牛们要到太空去了！他们打算建造一座太空电梯来送他们进入轨道。  
有 $k$ 种方块，第 $i$ 种有一个特定的高度 $h_i$，一定的存量 $c_i$. 为防宇宙射线的破坏，第 $i$ 种方块的任何部分不能超过高度 $a_i$。请用这些方块堆出最高的太空电梯。

## 输入格式
* Line $1$: A single integer, $k$.
* Lines $2 \ldots k+1$: Each line contains three space-separated integers: $h_i,a_i$, and $c_i$. Line $i+1$ describes block type $i$.
* 第一行输入一个整数 $k$。
* 接下来 $k$ 行，每行输入三个整数 $h_i,a_i,c_i$。
## 输出格式
* Line $1$: A single integer $h$, the maximum height of a tower that can be built.
* 一个整数，表示最大高度。
```input1
3
7 40 3
5 23 8
2 52 6
```
```output1
48
```
## 样例说明
从底部开始，先放 $3$ 个方块 $2$，之后 $3$ 个方块 $1$，接下来 $6$ 个方块 $3$。不能把 $3$ 个方块 $1$ 堆到 $4$ 个方块 $2$ 上，因为这样最高的方块 $1$ 的顶部高度超过了 $40$。
## 数据规模与约定
对于 $100\%$ 的数据，$1 \leq k \leq 400$，$1 \leq h_i \leq 100$，$1 \leq c_i \leq 10$，$1 \leq a_i \leq 4\times 10^4$。
## 题目来源
Gold