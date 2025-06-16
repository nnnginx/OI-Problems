# AT_icpc2013summer_warmingUp_i Topology

## 题目描述

[problemUrl]: https://atcoder.jp/contests/jag2013summer-warmingup/tasks/icpc2013summer_warmingUp_i

KM discovered that the number of holes is very important for some geometrical problems. He wants to calculate the number of holes of various figures. To simplify this problem, he assumes that the figures are composed of some unit squares whose vertices are on lattice points.  
 He can calculate it when the number of the squares is small. He can't calculate it by hand when the number is large, so he asks you, the friend of him and the excellent programmer, to solve this problem by computers.

 ![](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_icpc2013summer_warmingUp_i/c17d43c6db7c985b8cb351fe3f206176e2a0437f.png)Figure 1: Holes

 

 A hole is a bounded connected component when all squares are removed. When two components share some edges, they are considered connected.  
 The first line of the input file contains $ N $ ($ 1\ \leq\ N\ \leq\ 10^5 $), which is the number of squares.  
 Each of the following $ N $ lines describes a square by specifying integers $ X $ and $ Y $ ($ |X|,\ |Y|\ \leq\ 10^9 $) separated by single blank characters. $ X $ and $ Y $ are coordinates of the lower left corner.  
 You can assume that any two coordinates are different.  
 Output the number of the holes that the figure has.  
```

4
0 0
1 -1
2 0
1 1
```

 ```

1
```

 ```

16
1 0
3 0
5 0
0 1
2 1
4 1
1 2
3 2
4 2
1 3
5 3
0 4
1 4
2 4
4 4
3 5
```

 ```

3
```

## 输入格式

无

## 输出格式

无