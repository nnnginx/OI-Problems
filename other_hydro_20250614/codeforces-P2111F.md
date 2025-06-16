## Description

<div><p>You have been gifted a puzzle, where each piece of this puzzle is a square with a side length of one. You can glue any picture onto this puzzle, cut it, and obtain an almost ordinary jigsaw puzzle.</p><p>Your friend is an avid mathematician, so he suggested you consider the following problem. Is it possible to arrange the puzzle pieces in such a way that the following conditions are met:</p><ul> <li> the pieces are aligned parallel to the coordinate axes; </li><li> the pieces do not overlap each other; </li><li> all pieces form a single connected component (i.e., there exists a path from each piece to every other piece along the pieces, where each two consecutive pieces share a side); </li><li> the ratio of the perimeter of this component to the area of this component equals $\frac{p}{s}$; </li><li> the number of pieces used does not exceed $50\,000$. </li></ul><p>Can you handle it?</p><center> <img class="tex-graphics" src="./37707/file/fthZgO8f.png" style="zoom: 30.0%;max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">For this figure, the ratio of the perimeter to the area is $\frac{11}{9}$</span> </center></div><div class="input-specification"><p>Each test consists of several test cases. The first line contains a single integer $t$ ($1 \le t \le 10$)&nbsp;¡ª the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains two integers $p$ and $s$ ($1 \le p, s \le 50$).</p></div><div class="output-specification"><p>For each test case:</p><ul> <li> if it is impossible to arrange the pieces as described above, output a single integer $-1$; </li><li> otherwise, in the first line output a single integer $k$ ($1 \le k \le 50\,000$), and then in $k$ lines output the coordinates of the pieces: each line should contain two integers $x_{i}$ and $y_{i}$ ($-10^{9} \le x_{i}, y_{i} \le 10^{9}$). If there are multiple suitable arrangements of the pieces, output any of them. </li></ul></div>

## Input

<p>Each test consists of several test cases. The first line contains a single integer $t$ ($1 \le t \le 10$)&nbsp;¡ª the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains two integers $p$ and $s$ ($1 \le p, s \le 50$).</p>

## Output

<p>For each test case:</p><ul> <li> if it is impossible to arrange the pieces as described above, output a single integer $-1$; </li><li> otherwise, in the first line output a single integer $k$ ($1 \le k \le 50\,000$), and then in $k$ lines output the coordinates of the pieces: each line should contain two integers $x_{i}$ and $y_{i}$ ($-10^{9} \le x_{i}, y_{i} \le 10^{9}$). If there are multiple suitable arrangements of the pieces, output any of them. </li></ul>





```input1|2
2
1 1
31 4
```




```input2|2
2
4 2
12 5
```




```output1
20
3 7
3 8
6 4
6 5
3 5
4 4
4 5
4 3
3 4
5 3
5 4
5 7
3 6
4 6
5 5
5 6
4 7
4 8
6 6
6 7
-1
```




```output2
24
-7 2
-3 -3
-7 -5
-7 1
-3 2
-7 -2
-3 -5
-7 -6
-5 -6
-3 -4
-3 -6
-7 0
-6 -6
-7 -3
-5 2
-7 -1
-3 1
-4 -6
-3 0
-7 -4
-6 2
-4 2
-3 -1
-3 -2
5
0 0
0 1
1 0
-1 0
0 -1
```



## Note

<p>In the first test case of the first test, the figure may look like this:</p><center> <img class="tex-graphics" src="./37707/file/DwOihJK9.png" style="zoom: 50.0%;max-width: 100.0%;max-height: 100.0%;">   </center><p>In the second test, the figures look like this:</p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-left"><img class="tex-graphics" src="./37707/file/cy6z0KRN.png" style="zoom: 50.0%;max-width: 100.0%;max-height: 100.0%;"></td><td class="tex-tabular-text-align-left"><img class="tex-graphics" src="./37707/file/USeAC5bu.png" style="zoom: 50.0%;max-width: 100.0%;max-height: 100.0%;"></td></tr></tbody></table> </center><p>Note that the internal perimeter is also taken into account!</p>
