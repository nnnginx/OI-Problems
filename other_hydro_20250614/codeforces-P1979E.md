## Description

<div><p>The Manhattan distance between two points $(x_1, y_1)$ and $(x_2, y_2)$ is defined as: $$|x_1 - x_2| + |y_1 - y_2|.$$</p><p>We call a <span class="tex-font-style-it">Manhattan triangle</span> three points on the plane, the Manhattan distances between each pair of which are equal.</p><p>You are given a set of pairwise distinct points and an <span class="tex-font-style-bf">even</span> integer $d$. Your task is to find any Manhattan triangle, composed of three distinct points from the given set, where the Manhattan distance between any pair of vertices is equal to $d$.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $d$ ($3 \le n \le 2 \cdot 10^5$, $2 \le d \le 4 \cdot 10^5$, $d$ is even)&nbsp;！ the number of points and the required Manhattan distance between the vertices of the triangle.</p><p>The $(i + 1)$-th line of each test case contains two integers $x_i$ and $y_i$ ($-10^5 \le x_i, y_i \le 10^5$)&nbsp;！ the coordinates of the $i$-th point. It is guaranteed that all points are pairwise distinct.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output three distinct integers $i$, $j$, and $k$ ($1 \le i,j,k \le n$)&nbsp;！ the indices of the points forming the Manhattan triangle. If there is no solution, output "$0\ 0\ 0$" (without quotes).</p><p>If there are multiple solutions, output any of them.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $d$ ($3 \le n \le 2 \cdot 10^5$, $2 \le d \le 4 \cdot 10^5$, $d$ is even)&nbsp;！ the number of points and the required Manhattan distance between the vertices of the triangle.</p><p>The $(i + 1)$-th line of each test case contains two integers $x_i$ and $y_i$ ($-10^5 \le x_i, y_i \le 10^5$)&nbsp;！ the coordinates of the $i$-th point. It is guaranteed that all points are pairwise distinct.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output three distinct integers $i$, $j$, and $k$ ($1 \le i,j,k \le n$)&nbsp;！ the indices of the points forming the Manhattan triangle. If there is no solution, output "$0\ 0\ 0$" (without quotes).</p><p>If there are multiple solutions, output any of them.</p>





```input1|2,3,4,5,6,7,8,15,16,17,18,19,20,21,27,28,29,30,31,32,33,34,35,36,37
6
6 4
3 1
0 0
0 -2
5 -3
3 -5
2 -2
5 4
0 0
0 -2
5 -3
3 -5
2 -2
6 6
3 1
0 0
0 -2
5 -3
3 -5
2 -2
4 4
3 0
0 3
-3 0
0 -3
10 8
2 1
-5 -1
-4 -1
-5 -3
0 1
-2 5
-4 4
-4 2
0 0
-4 1
4 400000
100000 100000
-100000 100000
100000 -100000
-100000 -100000
```




```output1
2 6 1
4 3 5
3 5 1
0 0 0
6 1 3
0 0 0
```



## Note

<p>In the first test case:</p><center> <img class="tex-graphics" src="./34705/file/nL9UkcBE.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">Points $A$, $B$, and $F$ form a Manhattan triangle, the Manhattan distance between each pair of vertices is $4$. Points $D$, $E$, and $F$ can also be the answer.</span> </center><p>In the third test case:</p><center> <img class="tex-graphics" src="./34705/file/95DWAgSb.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">Points $A$, $C$, and $E$ form a Manhattan triangle, the Manhattan distance between each pair of vertices is $6$.</span> </center><p>In the fourth test case, there are no two points with a Manhattan distance of $4$, and therefore there is no suitable Manhattan triangle.</p>
