## 题目描述
FJ's cows really hate getting wet so much that the mere thought of getting caught in the rain makes them shake in their hooves. They have decided to put a rain siren on the farm to let them know when rain is approaching. They intend to create a rain evacuation plan so that all the cows can get to shelter before the rain begins. Weather forecasting is not always correct, though. In order to minimize false alarms, they want to sound the siren as late as possible while still giving enough time for all the cows to get to some shelter. The farm has $f \ (1 \le  f \le  200)$ fields on which the cows graze. A set of $p \ (1 \le  p \le  1500)$ paths connects them. The paths are wide, so that any number of cows can traverse a path in either direction. Some of the farm's fields have rain shelters under which the cows can shield themselves. These shelters are of limited size, so a single shelter might not be able to hold all the cows. Fields are small compared to the paths and require no time for cows to traverse. Compute the minimum amount of time before rain starts that the siren must be sounded so that every cow can get to some shelter.

约翰的牛们非常害怕淋雨，那会使他们瑟瑟发抖。他们打算安装一个下雨报警器，并且安排了一个撤退计划。他们需要计算最少的让所有牛进入雨棚的时间。牛们在农场的 $f$ 个田地上吃草。有 $p$ 条双向路连接着这些田地。路很宽，无限量的牛可以通过。田地上有雨棚，雨棚有一定的容量，牛们可以瞬间从这块田地进入这块田地上的雨棚请计算最少的时间，让每只牛都进入雨棚。
## 输入格式
* Line $1$: Two space-separated integers: $f$ and $p$.
* Lines $2\dots f+1$: Two space-separated integers that describe a field. The first integer (range: $0\dots 10^3$) is the number of cows in that field. The second integer (range: $0\dots 10^3$) is the number of cows the shelter in that field can hold. Line $i+1$ describes field $i$.
* Lines $f+2\dots f+p+1$: Three space-separated integers that describe a path. The first and second integers (both range $1\dots f$) tell the fields connected by the path. The third integer (range: $1\dots 10^9$) is how long any cow takes to traverse it.

* 第一行：两个整数 $f$ 和 $p$。
* 第二到 $f+1$ 行：第 $i+1$ 行有两个整数描述第 $i$ 个田地，第一个表示田地上的牛数，第二个表示田地上的雨棚容量。两个整数都在 $0$ 和 $10^3$ 之间。
* 第 $f+2$ 到 $f+p+1$ 行：每行三个整数描述一条路，分别是起点终点，及通过这条路所需的时间（在 $1$ 和 $10^9$ 之间）。
## 输出格式
* Line $1$: The minimum amount of time required for all cows to get under a shelter, presuming they plan their routes optimally. If it not possible for the all the cows to get under a shelter, output `-1`.

* 一个整数，表示最少的时间。如果无法使牛们全部进入雨棚，输出 `-1`。
```input1
3 4
7 2
0 4
2 6
1 2 40
3 2 70
2 3 90
1 3 120
```
```output1
110
```
## 样例说明
$1$ 号田的 $7$ 只牛中，$2$ 只牛直接进入 $1$ 号田的雨棚，$4$ 只牛进入 $1$ 号田的雨棚，$1$ 只进入 $3$ 号田的雨棚，加入其他的由 $3$ 号田来的牛们。所有的牛都能在 $110$ 单位时间内到达要去的雨棚。
## 数据规模与约定
对于 $100\%$ 的数据，$1 \leq f \leq 200$，$1 \leq p \leq 1500$。
## 题目来源
Gold