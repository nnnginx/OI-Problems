## 题目描述
地母是这个世界上大地的主宰，在她眼中整个大地呈现两行 $n$ 列这样一个状态（难不成她是对子眼?）。在这个大地上如珍珠般散落着各种宝藏，每个宝藏占据一个格子。不过这个消息让天公知道了，他想抢走这些宝藏。地母决定用「无极」牌帆布盖住这些宝藏。值得注意的是「无极」牌帆布全是矩形状的，而且地母现在手头比较紧，她决定用 $k$ 块帆布盖住所有的宝藏。现在希望你求出这 $k$ 块帆布的面积最小总和。
## 输入格式
* Line $1$: Three space-separated integers, $m,k$, and $n$.
* Lines $2\dots m+1$: Two space-separated integers in the range $(1,1)$ to $(2,n)$ giving the coordinates of the cell containing each cow. No cell contains more than one cow.
* 第一行给出三个数，分别代表宝藏的个数 $m$，帆布的张数 $k$，以及整个大地所呈现的列数 $n$，下面 $m$ 行给出两个数，代表每个宝藏所在的位置。
## 输出格式
* Line $1$: The minimum area required by the $k$ barns in order to cover all of the cows.
```input1
8 2 9
1 2
1 6
1 7
1 8
1 9
2 2
2 3
2 4
```
```output1
10
```
## 样例说明
INPUT DETAILS:   
As pictured above.

OUTPUT DETAILS:   
As discussed above.
## 数据规模与约定
对于 $100\%$ 的数据，$1 \le  n\le  1.5\times 10^7$，$1 \le  k\le m \le  10^3$。
## 题目来源
Gold