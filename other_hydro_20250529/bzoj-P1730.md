## 题目描述
Farmer John has $n \ (1 \le n \le 2.5\times 10^4)$ rectangular barns on his farm, all with sides parallel to the $x$ and $y$ axes and integer corner coordinates in the range $0\dots 10^6$. These barns do not overlap although they may share corners and/or sides with other barns. Since he has extra cows to milk this year, FJ would like to expand some of his barns. A barn has room to expand if it does not share a corner or a wall with any other barn. That is, FJ can expand a barn if all four of its walls can be pushed outward by at least some amount without bumping into another barn. If two barns meet at a corner, neither barn can expand. Please determine how many barns have room to expand.


约翰有 $n$ 个矩形牛棚，它们的墙均与坐标轴平行，而且其坐标在 $[0,10^6]$ 范围内。任意两个牛棚不重叠，但可能会有公共的墙。由于约翰的奶牛持续增加，他不得不考虑扩张牛棚。一个牛棚可以扩张，当且仅当它的四边均不与其它牛棚接触。如果两个牛棚有一个公共角，那它们均是不可扩张的。统计有多少牛棚可以扩张。
## 输入格式
* Line $1$：A single integer,$n$.
* Lines $2\dots n+1$：Four space-separated integers $a,b,c$, and $d$, describing one barn. The lower-left corner of the barn is at $\ (a,b)$ and the upper right corner is at $\ (c,d)$.

第一行输入 $n$，之后 $n$ 行每行输入一个牛棚的左下角和右上角坐标。

## 输出格式
* Line $1$：A single integer that is the number of barns that can be expanded.

输出可扩张的牛棚数。
```input1
5
0 2 2 7
3 5 5 8
4 2 6 4
6 1 8 6
0 0 8 1
```
```output1
2
```
## 样例说明
INPUT DETAILS：  
There are 5 barns. The first barn has its lower-left corner at $\ (0,2)$ and its upper-right corner at $\ (2,7)$, and so on.

仅有前两个牛棚可以扩张。

## 数据规模与约定
对于 $100\%$ 的数据，$1 \leq n \leq 2.5\times 10^4$。
## 题目来源
Gold