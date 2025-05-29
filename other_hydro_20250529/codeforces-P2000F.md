## Description

<div><p>You have $n$ rectangles, the $i$-th of which has a width of $a_i$ and a height of $b_i$.</p><p>You can perform the following operation an unlimited number of times: choose a rectangle and a cell in it, and then color it.</p><p>Each time you completely color any row or column, you earn $1$ point. Your task is to score at least $k$ points with as few operations as possible.</p><p>Suppose you have a rectangle with a width of $6$ and a height of $3$. You can score $4$ points by coloring all the cells in any $4$ columns, thus performing $12$ operations.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 100$) �� the number of test cases. The following are the descriptions of the test cases.</p><p>The first line of each test case description contains two integers $n$ and $k$ ($1 \le n \le 1000, 1 \le k \le 100$) �� the number of rectangles in the case and the required number of points.</p><p>The next $n$ lines contain the descriptions of the rectangles. The $i$-th line contains two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le 100$) �� the width and height of the $i$-th rectangle.</p><p>It is guaranteed that the sum of the values of $n$ across all test cases does not exceed $1000$.</p></div><div class="output-specification"><p>For each test case, output a single integer �� the minimum number of operations required to score at least $k$ points. If it is impossible to score at least $k$ points, output <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 100$) �� the number of test cases. The following are the descriptions of the test cases.</p><p>The first line of each test case description contains two integers $n$ and $k$ ($1 \le n \le 1000, 1 \le k \le 100$) �� the number of rectangles in the case and the required number of points.</p><p>The next $n$ lines contain the descriptions of the rectangles. The $i$-th line contains two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le 100$) �� the width and height of the $i$-th rectangle.</p><p>It is guaranteed that the sum of the values of $n$ across all test cases does not exceed $1000$.</p>

## Output

<p>For each test case, output a single integer �� the minimum number of operations required to score at least $k$ points. If it is impossible to score at least $k$ points, output <span class="tex-font-style-tt">-1</span>.</p>





```input1|2,3,6,7,8,9,10,11,15,16,17,18,23,24,25,26,27
7
1 4
6 3
1 5
4 4
5 10
1 1
1 1
1 1
1 1
1 1
2 100
1 2
5 6
3 11
2 2
3 3
4 4
3 25
9 2
4 3
8 10
4 18
5 4
8 5
8 3
6 2
```




```output1
12
14
5
-1
17
80
35
```


