## 题目描述
Bessie wants to navigate her spaceship through a dangerous asteroid field in the shape of an $n \times n$ grid $\ (1 \le  n \le  500)$. The grid contains $k$ asteroids $\ (1 \le  k \le  10^4)$, which are conveniently located at the lattice points of the grid. Fortunately, Bessie has a powerful weapon that can vaporize all the asteroids in any given row or column of the grid with a single shot. This weapon is quite expensive, so she wishes to use it sparingly. Given the location of all the asteroids in the field, find the minimum number of shots Bessie needs to fire to eliminate all of the asteroids.

贝茜想驾驶她的飞船穿过危险的小行星群。小行星群是一个 $n\times n$ 的网格，在网格内有 $k$ 个小行星。幸运地是贝茜有一个很强大的武器，一次可以消除所有在一行或一列中的小行星，这种武器很贵，所以她希望尽量地少用。给出所有的小行星的位置，算出贝茜最少需要多少次射击就能消除所有的小行星。
## 输入格式
* Line $1$: Two integers $n$ and $k$, separated by a single space.
* Lines $2\dots k+1$: Each line contains two space-separated integers $r$ and $c \ (1 \le  r, c \le  n)$ denoting the row and column coordinates of an asteroid, respectively.
* 第一行：两个整数 $n$ 和 $k$，用一个空格隔开。
* 第二行至 $k+1$ 行：每一行有两个空格隔开的整数 $r,c$，分别表示小行星所在的行和列。
## 输出格式
* Line $1$: The integer representing the minimum number of times Bessie must shoot.
* 一个整数表示贝茜需要的最少射击次数，可以消除所有的小行星。
```input1
3 4
1 1
1 3
2 2
3 2
```
```output1
2
```
## 样例说明
INPUT DETAILS:  
The following diagram represents the data, where `X` is an asteroid and `.` is empty space:  
```
X.X
.X.
.X.
```
OUTPUT DETAILS:  
Bessie may fire across row $1$ to destroy the asteroids at $(1,1)$ and$(1,3)$, and then she may fire down column $2$ to destroy the asteroids at $(2,2)$ and $(3,2)$.

## 数据规模与约定
对于 $100\%$ 的数据，$1 \leq n \leq 500$，$1 \leq k \leq 10^4$，$1 \leq r,c \leq n$。
## 题目来源
Gold