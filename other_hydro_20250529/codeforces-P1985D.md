## Description

<div><p>Given a $n$ by $m$ grid consisting of '.' and '#' characters, there exists a whole manhattan circle on the grid. The top left corner of the grid has coordinates $(1,1)$, and the bottom right corner has coordinates $(n, m)$.</p><p>Point ($a, b$) belongs to the manhattan circle centered at ($h, k$) if $|h - a| + |k - b| &lt; r$, where $r$ is a positive constant.</p><p>On the grid, the set of points that are part of the manhattan circle is marked as '#'. Find the coordinates of the center of the circle.</p></div><div class="input-specification"><p>The first line contains $t$ ($1 \leq t \leq 1000$) &nbsp;！ the number of test cases.</p><p>The first line of each test case contains $n$ and $m$ ($1 \leq n \cdot m \leq 2 \cdot 10^5$)&nbsp;！ the height and width of the grid, respectively. </p><p>The next $n$ lines contains $m$ characters '.' or '#'. If the character is '#', then the point is part of the manhattan circle.</p><p>It is guaranteed the sum of $n \cdot m$ over all test cases does not exceed $2 \cdot 10^5$, and there is a whole manhattan circle on the grid.</p></div><div class="output-specification"><p>For each test case, output the two integers, the coordinates of the center of the circle.</p></div>

## Input

<p>The first line contains $t$ ($1 \leq t \leq 1000$) &nbsp;！ the number of test cases.</p><p>The first line of each test case contains $n$ and $m$ ($1 \leq n \cdot m \leq 2 \cdot 10^5$)&nbsp;！ the height and width of the grid, respectively. </p><p>The next $n$ lines contains $m$ characters '.' or '#'. If the character is '#', then the point is part of the manhattan circle.</p><p>It is guaranteed the sum of $n \cdot m$ over all test cases does not exceed $2 \cdot 10^5$, and there is a whole manhattan circle on the grid.</p>

## Output

<p>For each test case, output the two integers, the coordinates of the center of the circle.</p>





```input1|2,3,4,5,6,7,14,15,16,17,18,19,22,23,24,25,26,27
6
5 5
.....
.....
..#..
.....
.....
5 5
..#..
.###.
#####
.###.
..#..
5 6
......
......
.#....
###...
.#....
1 1
#
5 6
...#..
..###.
.#####
..###.
...#..
2 10
..........
...#......
```




```output1
3 3
3 3
4 2
1 1
3 4
2 4
```


