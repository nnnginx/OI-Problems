## Description

<div><p>You are given $n$ sticks of lengths $a_1, a_2, \ldots, a_n$. Find the maximum number of regular (equal-sided) polygons you can construct simultaneously, such that: </p><ul> <li> Each side of a polygon is formed by exactly one stick. </li><li> No stick is used in more than $1$ polygon. </li></ul><p>Note: Sticks cannot be broken.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 100$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 100$)&nbsp;！ the number of sticks available.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 100$)&nbsp;！ the stick lengths.</p></div><div class="output-specification"><p>For each test case, output a single integer on a new line&nbsp;！ the maximum number of regular (equal-sided) polygons you can make simultaneously from the sticks available.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 100$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 100$)&nbsp;！ the number of sticks available.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 100$)&nbsp;！ the stick lengths.</p>

## Output

<p>For each test case, output a single integer on a new line&nbsp;！ the maximum number of regular (equal-sided) polygons you can make simultaneously from the sticks available.</p>





```input1|2,3,6,7
4
1
1
2
1 1
6
2 2 3 3 3 3
9
4 2 2 2 2 4 2 4 4
```




```output1
0
0
1
2
```



## Note

<p>In the first test case, we only have one stick, hence we can't form any polygon.</p><p>In the second test case, the two sticks aren't enough to form a polygon either.</p><p>In the third test case, we can use the $4$ sticks of length $3$ to create a square.</p><p>In the fourth test case, we can make a pentagon with side length $2$, and a square of side length $4$.</p>
