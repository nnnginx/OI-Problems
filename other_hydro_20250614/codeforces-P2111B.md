## Description

<div><p>There are $n$ Fibonacci cubes, where the side of the $i$-th cube is equal to $f_{i}$, where $f_{i}$ is the $i$-th Fibonacci number.</p><p>In this problem, the Fibonacci numbers are defined as follows:</p><ul> <li> $f_{1} = 1$ </li><li> $f_{2} = 2$ </li><li> $f_{i} = f_{i - 1} + f_{i - 2}$ for $i &gt; 2$ </li></ul><p>There are also $m$ empty boxes, where the $i$-th box has a width of $w_{i}$, a length of $l_{i}$, and a height of $h_{i}$.</p><p>For each of the $m$ boxes, you need to determine whether all the cubes can fit inside that box. The cubes must be placed in the box following these rules:</p><ul> <li> The cubes can only be stacked in the box such that the sides of the cubes are parallel to the sides of the box; </li><li> Every cube must be placed either on the bottom of the box or on top of other cubes in such a way that all space below the cube is occupied; </li><li> A larger cube cannot be placed on top of a smaller cube. </li></ul></div><div class="input-specification"><p>Each test consists of several test cases. The first line contains a single integer $t$ ($1 \le t \le 10^{3}$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>In the first line of each test case, there are two integers $n$ and $m$ ($2 \le n \le 10, 1 \le m \le 2 \cdot 10^{5}$)&nbsp;！ the number of cubes and the number of empty boxes.</p><p>The next $m$ lines of each test case contain $3$ integers $w_{i}$, $l_{i}$, and $h_{i}$ ($1 \le w_{i}, l_{i}, h_{i} \le 150$)&nbsp;！ the dimensions of the $i$-th box.</p><p>Additional constraints on the input:</p><ul> <li> The sum of $m$ across all test cases does not exceed $2 \cdot 10^{5}$. </li></ul></div><div class="output-specification"><p>For each test case, output a string of length $m$, where the $i$-th character is equal to "<span class="tex-font-style-tt">1</span>" if all $n$ cubes can fit into the $i$-th box; otherwise, the $i$-th character is equal to "<span class="tex-font-style-tt">0</span>".</p></div>

## Input

<p>Each test consists of several test cases. The first line contains a single integer $t$ ($1 \le t \le 10^{3}$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>In the first line of each test case, there are two integers $n$ and $m$ ($2 \le n \le 10, 1 \le m \le 2 \cdot 10^{5}$)&nbsp;！ the number of cubes and the number of empty boxes.</p><p>The next $m$ lines of each test case contain $3$ integers $w_{i}$, $l_{i}$, and $h_{i}$ ($1 \le w_{i}, l_{i}, h_{i} \le 150$)&nbsp;！ the dimensions of the $i$-th box.</p><p>Additional constraints on the input:</p><ul> <li> The sum of $m$ across all test cases does not exceed $2 \cdot 10^{5}$. </li></ul>

## Output

<p>For each test case, output a string of length $m$, where the $i$-th character is equal to "<span class="tex-font-style-tt">1</span>" if all $n$ cubes can fit into the $i$-th box; otherwise, the $i$-th character is equal to "<span class="tex-font-style-tt">0</span>".</p>





```input1|2,3,4,5,6
2
5 4
3 1 2
10 10 10
9 8 13
14 7 20
2 6
3 3 3
1 2 1
2 1 2
3 2 2
2 3 1
3 2 4
```




```output1
0010
100101
```



## Note

<p>In the first test case, only one box is suitable. The cubes can be placed in it as follows:</p><center> <img class="tex-graphics" src="./37711/file/PsPfGCRm.png" style="zoom: 70.0%;max-width: 100.0%;max-height: 100.0%;"> </center>
