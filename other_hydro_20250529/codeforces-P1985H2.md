## Description

<div><p><span class="tex-font-style-bf">Easy and hard versions are actually different problems, so read statements of both problems completely and carefully. The only difference between the two versions is the operation.</span></p><p>Alex has a grid with $n$ rows and $m$ columns consisting of '<span class="tex-font-style-tt">.</span>' and '<span class="tex-font-style-tt">#</span>' characters. A set of '<span class="tex-font-style-tt">#</span>' cells forms a connected component if from any cell in this set, it is possible to reach any other cell in this set by only moving to another cell in the set that shares a <span class="tex-font-style-bf">common side</span>. The size of a connected component is the number of cells in the set.</p><p>In one operation, Alex selects any row $r$ ($1 \le r \le n$) <span class="tex-font-style-bf">and</span> any column $c$ ($1 \le c \le m$), then sets every cell in row $r$ <span class="tex-font-style-bf">and</span> column $c$ to be '<span class="tex-font-style-tt">#</span>'. Help Alex find the maximum possible size of the largest connected component of '<span class="tex-font-style-tt">#</span>' cells that he can achieve after performing the operation <span class="tex-font-style-bf">at most once</span>.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \leq t \leq 10^4$) ！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n \cdot m \le 10^6$) ！ the number of rows and columns of the grid.</p><p>The next $n$ lines each contain $m$ characters. Each character is either '<span class="tex-font-style-tt">.</span>' or '<span class="tex-font-style-tt">#</span>'.</p><p>It is guaranteed that the sum of $n \cdot m$ over all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, output a single integer ！ the maximum possible size of a connected component of '<span class="tex-font-style-tt">#</span>' cells that Alex can achieve.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \leq t \leq 10^4$) ！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n \cdot m \le 10^6$) ！ the number of rows and columns of the grid.</p><p>The next $n$ lines each contain $m$ characters. Each character is either '<span class="tex-font-style-tt">.</span>' or '<span class="tex-font-style-tt">#</span>'.</p><p>It is guaranteed that the sum of $n \cdot m$ over all test cases does not exceed $10^6$.</p>

## Output

<p>For each test case, output a single integer ！ the maximum possible size of a connected component of '<span class="tex-font-style-tt">#</span>' cells that Alex can achieve.</p>





```input1|2,3,9,10,11,12,19,20,21,22,23,24,25
6
1 1
.
4 2
..
#.
#.
.#
3 5
.#.#.
..#..
.#.#.
5 5
#...#
....#
#...#
.....
...##
6 6
.#..#.
#..#..
.#...#
#.#.#.
.#.##.
###..#
6 8
..#....#
.####.#.
###.#..#
.##.#.##
.#.##.##
#..##.#.
```




```output1
1
7
11
16
22
36
```



## Note

<p>In the fourth test case, it is optimal for Alex to set all cells in row $4$ and column $2$ to be '<span class="tex-font-style-tt">#</span>'. Doing so will lead to the largest connected component of '<span class="tex-font-style-tt">#</span>' having a size of $16$.</p><p>In the fifth test case, it is optimal for Alex to set all cells in row $2$ and column $4$ to be '<span class="tex-font-style-tt">#</span>'. Doing so will lead to the largest connected component of '<span class="tex-font-style-tt">#</span>' having a size of $22$.</p>
