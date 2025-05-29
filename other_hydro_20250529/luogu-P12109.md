## 题目背景
*Looking at problems `K-Shaped Figures` and `H-Shaped Figures` from the past two years, you took the warning seriously. You came prepared. For each of the remaining 24 letters of the alphabet, you theorized what the problem could be. You even implemented all 24 solutions and used up all of your Digital Team Reference Document space just to bring these codes to the contest. If the judges are so unoriginal that they set another problem about letter shapes, you'll just get it accepted on minute 1 and leave everyone puzzled.*

*What, another shapes problem? Really?! Ha-ha! Oh... wait a second...*

## 题目描述
Let's say that two circles on a plane form an $\textit{8-shaped figure}$ if they touch each other, but neither of them lies inside the other one.

![](https://cdn.luogu.com.cn/upload/image_hosting/selhsqb5.png)

You are given a collection of $n$ circles on the plane. No two circles have more than one common point. In other words, no two circles intersect twice or coincide, but they can touch or lie one within another.

Find the number of pairs of circles from this collection that form an 8-shaped figure.

## 输入格式
Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.

The first line of each test case contains a single integer $n$, denoting the number of circles ($2 \le n \le 2 \cdot 10^5$).
 
The $i$-th of the following $n$ lines contains three integers $x_i$, $y_i$, and $r_i$, denoting the coordinates of the center of the $i$-th circle and its radius ($-10^9 \le x_i, y_i \le 10^9$; $1 \le r_i \le 10^9$). No two circles intersect twice or coincide, but they can touch or lie one within another.

It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.

## 输出格式
For each test case, print the number of pairs of circles that form an 8-shaped figure.


```input1
2
5
1 1 1
1 3 1
3 1 1
3 3 1
6 7 4
6
-3 0 3
-2 0 2
-1 0 1
1 0 1
2 0 2
3 0 3
```

```output1
5
9
```

