## 题目描述
One of the farming chores Farmer John dislikes the most is hauling around lots of cow manure. In order to streamline this process, he comes up with an intriguing idea: instead of hauling manure between two points in a cart behind his tractor, why not shoot it through the air with a giant manure slingshot? (indeed, what could possibly go wrong...)
Farmer John's farm is built along a single long straight road, so any location on his farm can be described simply using its position along this road (effectively a point on the number line). FJ builds $N$ slingshots ($1 \leq N \leq 10^5$), where the $i$th slingshot is described by three integers $x_i$, $y_i$, and $t_i$, specifying that this slingshot can shoot manure from position $x_i$ to position $y_i$ in only $t_i$ total units of time.

FJ has $M$ piles of manure to transport ($1 \leq M \leq 10^5$). The $j$th such pile needs to be moved from position $a_j$ to position $b_j$. Hauling manure with the tractor for a distance of $d$ takes $d$ units of time. FJ is hoping to reduce this by allowing up to one use of any slingshot for transporting each pile of manure. Time FJ spends moving his tractor without manure in it does not count.

For each of the $M$ manure piles, please help FJ determine the minimum possible transportation time, given that FJ can use up to one slingshot during the process.

## 输入格式
The first line of input contains $N$ and $M$. The next $N$ lines each describe a single slingshot in terms of integers $x_i$, $y_i$, and $t_i$ ($0 \leq x_i, y_i, t_i \leq 10^9$). The final $M$ lines describe piles of manure that need to be moved, in terms of integers $a_j$ and $b_j$.

## 输出格式
Print $M$ lines of output, one for each manure pile, indicating the minimum time needed to transport it.

## 题目大意
### 题目描述

Farmer John 最不喜欢的农活之一就是到处搬运牛粪。为了简化这一过程，他想出了一个有趣的主意：与其用拖拉机后面的拖车搬运牛粪，为什么不通过一个巨大的牛粪弹弓将其射到空中呢？（确实，可能会出什么问题呢……）

Farmer John 的农场建在一条笔直的长路上，因此农场上的任何位置都可以简单地用其在这条路上的位置来描述（实际上就是数轴上的一个点）。FJ 建造了 $N$ 个弹弓（$1 \leq N \leq 10^5$），其中第 $i$ 个弹弓由三个整数 $x_i$、$y_i$ 和 $t_i$ 描述，表示这个弹弓可以将牛粪从位置 $x_i$ 射到位置 $y_i$，仅需 $t_i$ 个单位时间。

FJ 有 $M$ 堆牛粪需要搬运（$1 \leq M \leq 10^5$）。第 $j$ 堆牛粪需要从位置 $a_j$ 搬运到位置 $b_j$。用拖拉机搬运牛粪，每移动距离 $d$ 需要 $d$ 个单位时间。FJ 希望通过允许每堆牛粪最多使用一次弹弓来减少搬运时间。FJ 在没有牛粪的情况下移动拖拉机的时间不计入搬运时间。

对于每堆牛粪，请帮助 FJ 确定在最多使用一次弹弓的情况下，搬运所需的最少时间。

### 输入格式

输入的第一行包含 $N$ 和 $M$。接下来的 $N$ 行每行描述一个弹弓，包含三个整数 $x_i$、$y_i$ 和 $t_i$（$0 \leq x_i, y_i, t_i \leq 10^9$）。最后的 $M$ 行描述需要搬运的牛粪堆，每行包含两个整数 $a_j$ 和 $b_j$。

### 输出格式

输出 $M$ 行，每行对应一堆牛粪，表示搬运所需的最少时间。

### 提示

在这里，第一堆牛粪需要从位置 $1$ 搬运到位置 $12$。如果不使用弹弓，这将花费 $11$ 个单位时间。然而，使用第一个弹弓，花费 $1$ 个单位时间将牛粪移动到位置 $0$（弹弓的起点），$1$ 个单位时间将牛粪射到位置 $10$（弹弓的终点），然后花费 $2$ 个单位时间将牛粪移动到位置 $12$。第二堆牛粪最好不使用弹弓搬运，而第三堆牛粪应使用第二个弹弓搬运。

题目来源：Brian Dean

```input1
2 3
0 10 1
13 8 2
1 12
5 2
20 7
```

```output1
4
3
10
```

## 提示
Here, the first pile of manure needs to move from position 1 to position 12. Without using an slingshot, this would take 11 units of time. However, using the first slingshot, it takes 1 unit of time to move to position 0 (the slingshot source), 1 unit of time to fling the manure through the air to land at position 10 (the slingshot destination), and then 2 units of time to move the manure to position 12. The second pile of manure is best moved without any slingshot, and the third pile of manure should be moved using the second slingshot.

Problem credits: Brian Dean

