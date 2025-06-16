## 题目描述
Bessie and the rest of Farmer John's cows are taking a trip this winter to go skiing. One day Bessie finds herself at the top left corner of an $r \ (1 \le  r \le  100)$ by $c \ (1 \le  c \le  100)$ grid of elevations $e \ (-25 \le  e \le  25)$. In order to join FJ and the other cows at a discow party, she must get down to the bottom right corner as quickly as she can by travelling only north, south, east, and west. Bessie starts out travelling at a initial speed $v \ (1 \le  v \le  10^6)$. She has discovered a remarkable relationship between her speed and her elevation change. When Bessie moves from a location of height $a$ to an adjacent location of height $b$, her speed is multiplied by the number $2^{a-b}$. The time it takes Bessie to travel from a location to an adjacent location is the reciprocal of her speed when she is at the first location. Find the both smallest amount of time it will take Bessie to join her cow friends and the number of moves required by the path (a move is a transition from one location to another adjacent location).

贝茜和其他一些人去滑雪。贝茜发现她自己站在一块 $r \times c$ 的区域中，区域中的每一块都有一个高度值 $e_{i,j}$。为了参加大家的聚会，贝茜想要尽快到达右下角。贝茜每一步只能向正东，正西，正南，正北前进一步。贝茜以初速度 $v$ 前进，她发现了一个她的速度和高度的关系。当贝茜从高度 $a$ 移动到高度 $b$，她的速度就乘上了一个数 $2^{a-b}$。贝茜移动一步的速度取决于她在前一格时的速度。请找出贝茜移动所需的最小时间。
## 输入格式
* Line $1$: Three space-separated integers: $v,r$, and $c$, which respectively represent Bessie's initial velocity and the number of rows and columns in the grid.
* Lines $2\dots r+1$: $c$ integers representing the elevation $e$ of the corresponding location on the grid.
* 第一行：$3$ 个用空格隔开的整数 $v,r,c$，分别表示贝茜的初速度和区域的长度和宽度。
* 第二到 $r+1$ 行：以矩阵的形式表示该区域中各块的高度。
## 输出格式
A single number value, printed to two exactly decimal places: the minimum amount of time that Bessie can take to reach the bottom right corner of the grid.  
输出一个实数（**保留 $2$ 位小数**），表示贝茜达到目的地最少需要的时间。
```input1
1 3 3
1 5 3
6 3 5
2 4 3
```
```output1
29.00
```
## 样例说明
奶牛开始在左上角，速度为 $1$，它可以移动到别的格子上，速度会发生变化。  
$3\times 3$ 的数矩阵代表每个格子的参数，当从一个格子 $a$ 到 $b$ 时，速度变成 $v\times 2^{a-b}$。

OUTPUT DETAILS:  
Bessie's best route is:  
Start at $\ (1,1)$ time $0$ speed $1$.  
East to $\ (1,2)$ time $1$ speed $\dfrac{1}{16}$.  
South to $\ (2,2)$ time $17$ speed $\dfrac{1}{4}$.  
South to $\ (3,2)$ time $21$ speed $\dfrac{1}{8}$.  
East to $\ (3,3)$ time $29$ speed $\dfrac{1}{4}$.  
## 数据规模与约定
对于 $100\%$ 的数据，$1 \leq r,c \leq 100$，$-25 \le  e_{i,j} \le  25$，$1 \leq v \leq 10^6$。
## 题目来源
Gold