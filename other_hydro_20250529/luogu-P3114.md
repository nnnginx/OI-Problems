## 题目描述
Farmer John's N cows (1 <= N <= 50,000) appear to be stampeding along the road at the front of FJ's farm, but they are actually just running in a foot race to see which cow is the fastest.

Viewed from above, each cow is represented by a unit-length horizontal line segment, specified by the coordinates of its left corner point at time t=0.  For example, (-3,6) would specify a cow who at time t=0 is represented by the segment from (-3,6) to (-2,6).  Each cow is moving to the right (in the +x direction) at a certain rate, specified by the integer amount of time it takes her to move 1 unit to the right.

FJ is not particularly thrilled that his cows are outside running instead of in the barn producing milk.  He plans to admonish them with a stern lecture after the race ends.  In order to determine which of his cows are participating in the race, FJ situates himself at (0,0) and looks along a ray extending in the +y direction.  As the race unfolds, FJ sees a cow if she is ever the first cow visible along this ray.  That is, a cow might not be visible if another cow is "in front" of her during the entire time she crosses FJ's line of sight.

Please compute the number of cows FJ can see during the entire race.

## 输入格式
INPUT:

The first line of the input contains N.  Each of the following N lines describes a cow with three integers x y r, corresponding to a cow whose left endpoint is at (x,y) at time t=0, moving to the right at a continuous speed of 1 unit of distance every r units of time.  The value of x is in the range -1000..-1, the value of y is in the range 1..1,000,000 (and distinct for every cow, to prevent any possible collisions), and the value of r is in the range 1..1,000,000. 

## 输出格式
OUTPUT:

A single integer, specifying the number of cows FJ can see during the entire race (from t=0 onward). 



## 题目大意
### 题目描述

FJ 的 $N$ 头奶牛（$1 \leq N \leq 50,000$）看似在农场前的路上狂奔，实际上它们正在进行一场赛跑。

从上方俯视，每头牛在时间 $t = 0$ 时被表示为一个单位长度的水平线段，其左端点坐标为 $(x, y)$。例如，$(-3, 6)$ 表示一头在 $t = 0$ 时从 $(-3, 6)$ 延伸到 $(-2, 6)$ 的奶牛。每头牛以一定速度向右（$+x$ 方向）移动，该速度由移动 1 单位距离所需的整数时间 $r$ 描述。

FJ 并不满意他的奶牛在外赛跑而不在牛棚产奶。他计划在比赛结束后训斥参赛的奶牛。为了确定哪些奶牛参赛，FJ 站在 $(0, 0)$ 处并沿 $+y$ 方向的射线观察。当一头牛在某个时刻成为这条射线上首个可见的牛时，FJ 就会看到它。如果一头牛在穿过 FJ 视线期间始终被其他牛"挡住"，则她不可见。

请计算 FJ 在整个比赛过程中能看到的奶牛数量。

### 输入格式

第一行包含 $N$。接下来 $N$ 行每行描述一头牛，包含三个整数 $x$ $y$ $r$，分别表示：左端点初始坐标为 $(x, y)$，以每移动 1 单位距离需要 $r$ 单位时间的速度向右移动。$x$ 的取值范围为 $-1000$ 到 $-1$，$y$ 的取值范围为 $1$ 到 $1,000,000$（所有牛的 $y$ 值互不相同以避免碰撞），$r$ 的取值范围为 $1$ 到 $1,000,000$。

### 输出格式
 
一个整数，表示 FJ 能看到的奶牛数量。

### 说明/提示

FJ 可以看到牛 1 和 2，但看不到牛 3。

```input1
3 
-2 1 3 
-3 2 3 
-5 100 1 

```

```output1
2 

```

## 提示
SOLUTION NOTES:

FJ can see cows 1 and 2 but not cow 3.



