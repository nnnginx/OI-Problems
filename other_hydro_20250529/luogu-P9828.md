## 题目描述

At the Namomo Camp, a cute volunteer celebrates her birthday. Wowo buys her a huge cake. (The cake is so big that it has a 3D coordinate system inside.) There are $n$ cuboid shaped pieces of chocolates $\textbf{in}$ the cake. The $i$-th ($1\le i\le n$) chocolate consists of all points $(x,y,z)$ such that $min\_x[i]\le x\le max\_x[i], min\_y[i]\le y\le max\_y[i], min\_z[i]\le z\le max\_z[i]$. $min\_x,max\_x, min\_y,max\_y, min\_z, max\_z$ are $6$ arrays of integers. Chocolates may overlap or touch each other.

The volunteer wants to distribute the cake to the campers of the Namomo Camp. To show off his knife skill, Wowo decides to cut the cake into pieces by exactly $3$ cuts such that:

- The first cut is a plane whose equation is $x=a$ for some integer $a$ decided by Wowo.
- The second cut is a plane whose equation is $y=b$ for some integer $b$ decided by Wowo.
- The third cut is a plane whose equation is $z=c$ for some integer $c$ decided by Wowo.
- Each chocolate is $\textbf{touched}$ by at least one cut (i.e. each cuboid has a nonempty intersection with at least one plane).

Decide whether Wowo can cut the cake under the rules. If the answer is yes, output any possible solution.

## 输入格式
The first line contains a single integer $n$ ($1\le n\le 100000$).

The $i$-th line of the next $n$ lines contains $6$ integers $min\_x[i],max\_x[i], min\_y[i],max\_y[i], min\_z[i], max\_z[i]$ ($-10^9\le min\_x[i],max\_x[i], min\_y[i],max\_y[i], min\_z[i], max\_z[i]\le 10^9$, $min\_x[i]<max\_x[i]$, $min\_y[i]<max\_y[i]$, $min\_z[i]< max\_z[i]$).

## 输出格式
If Wowo can cut the cake under the rules, the first line of the output should contain ``YES`` and the second line should contain $3$ integers $a$, $b$ and $c$ ($-10^9\le a, b, c\le 10^9$). If Wowo cannot cut the cake under the rules, output only one line containing ``NO``.

## 题目大意
有一个巨大的蛋糕，蛋糕里面有$n$块立方体形状的巧克力，每块巧克力的位置由它的对角线坐标定义。一个人想通过三个平面切割这个蛋糕，每个平面的方程分别是$x=a$，$y=b$和$z=c$，其中$a$、$b$和$c$是整数。目标是选择$a$、$b$和$c$这样每块巧克力至少被一个切割平面触及。

输入由一个整数$n$开始，表示巧克力的数量，后面跟着$n$行，每行六个整数，分别代表每块巧克力在三维坐标系中的最小和最大$x$、$y$、$z$坐标。

输出要求是如果存在这样的三个切割平面，第一行输出``YES``，第二行输出三个整数$a$、$b$和$c$。如果不存在，只输出``NO``。

```input1
3
0 1 0 1 0 1
10 11 10 11 10 11
999999999 1000000000 999999999 1000000000 999999999 1000000000
```

```output1
YES
0 10 999999999
```

```input2
4
0 1 0 1 0 1
999999999 1000000000 0 1 0 1
0 1 999999999 1000000000 0 1
0 1 0 1 999999999 1000000000
```

```output2
YES
0 0 0
```

