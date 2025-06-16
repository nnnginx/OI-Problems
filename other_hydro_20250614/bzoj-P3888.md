## 题目描述
Farmer John's $n$ cows appear to be stampeding along the road at the front of FJ's farm, but they are actually just running in a foot race to see which cow is the fastest. Viewed from above, each cow is represented by a unit-length horizontal line segment, specified by the coordinates of its left corner point at time $t=0$.For example, $(-3,6)$ would specify a cow who at time $t=0$ is represented by the segment from $(-3,6)$ to $(-2,6)$. Each cow is moving to the right (in the **+x** direction) at a certain rate, specified by the integer amount of time it takes her to move $1$ unit to the right. FJ is not particularly thrilled that his cows are outside running instead of in the barn producing milk. He plans to admonish them with a stern lecture after the race ends. In order to determine which of his cows are participating in the race, FJ situates himself at $(0,0)$ and looks along a ray extending in the **+y** direction. As the race unfolds, FJ sees a cow if she is ever the first cow visible along this ray. That is, a cow might not be visible if another cow is "in front" of her during the entire time she crosses FJ's line of sight. Please compute the number of cows FJ can see during the entire race.

**翻译：**

FJ 站在原点上向 $y$ 轴正半轴看，然后有一群羊驼从他眼前飞过。这些羊驼初始都在第二象限，尾巴在 $(x_i,y_i)$，头在 $(x_i+1,y_i)$，每 $c_i$ 秒向右走一个单位。FJ 能看见一匹羊驼当且仅当它身体任意某部位 $x$ 坐标为 $0$ 时，没有其它 $y$ 坐标小于此羊驼的羊驼身体某部位 $x$ 坐标为 $0$。问 FJ 能看见几匹羊驼？

## 输入格式
The first line of the input contains $n$. Each of the following $n$ lines describes a cow with three integers $x_i,y_i,c_i$,corresponding to a cow whose left endpoint is at $(x_i,y_i)$ at time $t=0$, moving to the right at a continuous speed of $1$ unit of distance every $c_i$ units of time. 

Distinct for every cow, to prevent any possible collisions

## 输出格式

A single integer, specifying the number of cows FJ can see during the entire race (from $t=0$ onward).

```input1
3
-2 1 3
-3 2 3
-5 100 1
```

```output1
2
```

## 样例说明

FJ can see cows $1$ and $2$ but not cow $3$.

## 数据规模与约定

对于 $100\%$ 的数据，$1\le n \le 5\times 10^4$，$-10^3\le x_i \le -1,1\le y_i \le 10^6,1\le c \le 10^6$。

## 题目来源

Silver & 鸣谢 PoPoQQQ