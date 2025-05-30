## 题目描述
Farmer John has purchased the world's most loathesome hay baler. Instead of having a drive-roller that drives maybe an idler roller that drives the power take-off for the baler, it has N rollers (2 <= N <= 1050) which drive and are driven by various rollers.

FJ has meticulously cataloged data for each roller i: X\_i,Y\_i are the center of the roller (-5000 <= X\_i <= 5000; -5000 <= Y\_i <= 5000); R\_i is the roller's radius (3 <= R\_i <= 800). The drive-roller is located at 0,0; the baler power take-off is located at X\_t,Y\_t (numbers supplied in the input).

The drive-roller turns clockwise at 10,000 revolutions per hour. Your job is to determine the speeds of all the rollers that are in the power-train: from the drive-roller through the power take-off roller. Rollers that do not transfer power to the take-off roller are to be ignored. A roller of radius Rd that is turning at S rph and driving another roller of radius Rx will cause the second roller to turn at the speed -S\*Rd/Rx (where the sign denotes whether the roller is turning clockwise or counterclockwise (anticlockwise for our British friends)).

Determine the power-train path and report the sum of the absolute values of all those rollers' speeds. All the rollers in the input set except the driver-roller are driven by some other roller; power is never transferred to a roller from more than one other roller.

Report your answer as an integer that is the truncated value after summing all the speeds.

## 输入格式
\* Line 1: Three space-separated integers: N, X\_t, and Y\_t

\* Lines 2..N+1: Line i+1 describes roller i's properties: X\_i, Y\_i, and R\_i

## 输出格式
\* Line 1: A single integer that is the truncated version of the sum of the absolute value of the speeds of the rollers in the power-train including the drive-roller, all the driven rollers, and the power take-off roller.

## 题目大意
Farmer John 新买的干草打包机的内部结构大概算世界上最混乱的了，它不像普通的机器一样有明确的内部传动装置，而是 $N$ 个齿轮互相作用，每个齿轮都可能驱动着多个齿轮。 FJ 记录了对于每个齿轮 $i$，记录了它的 $3$ 个参数，以一个三元组 $(x,y,r)$ 表示，$x$ 和 $y$ 表示齿轮中心的位置坐标，$r$ 表示该齿轮的半径。

驱动齿轮的位置为 $(0,0)$，并且 FJ 也知道最终的工作齿轮位于 $(X_t,Y_t)$。 驱动齿轮顺时针转动，转速为 $10,000$ 转/小时。你的任务是，确定传动序列中所有齿轮的转速。传动序列的定义为，能量由驱动齿轮传送到工作齿轮的过程中用到的所有齿轮的集合。对能量传送无意义的齿轮都应当被忽略。

在一个半径为 $R_d$，转速为 $S$ 转/每小时的齿轮的带动下，与它相接的半径为 $R_x$ 的齿轮的转速将为 $-S\times \frac{R_d}{R_x}$ 转/小时。$S$ 前的负号的意思是，一个齿轮带动的另一个齿轮的转向会与它的转向相反。

FJ 只对整个传动序列中所有齿轮速度的绝对值之和感兴趣，你的任务也就相应转化成求这个值。机器中除了驱动齿轮以外的所有齿轮都被另外某个齿轮带动，并且不会出现 $2$ 个不同的齿轮带动同一个齿轮的情况。

### 输入格式

第一行，三个整数，分别代表 $N,X_t,Y_t$；

第 $2$ 行到第 $N+1$ 行，每行三个整数，代表一个三元组 $(x,y,r)$。

### 输出格式

输出共一行，一个整数，代表整个传动序列中所有齿轮速度的绝对值之和。

```input1
4 32 54 
0 0 10 
0 30 20 
32 54 20 
-40 30 20 

```

```output1
20000 

```

## 提示
$2 \leq N \leq 1050$，$-5000 \leq x,y \leq 5000$，$3 \leq r \leq 800$。




Four rollers: the drive-roller at 0,0 with radius 10. It drives the roller above it at 0,30 with radius 20. That roller drives both the power take-off roller at 32,54 (r=20) and a random roller (not in the power train) at -40,30 (r=20).


Roller   Radius   Speed

1 (0,0)     10     10,000 

2 (0,30)    20     -5,000 

3 (32,54)   20      5,000 

------
Sum of abs values: 20,000


