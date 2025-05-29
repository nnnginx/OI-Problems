## Description

<div><p>Consider a set of points on a line. The distance between two points $i$ and $j$ is $|i - j|$.</p><p>The point $i$ from the set is <span class="tex-font-style-bf">the closest</span> to the point $j$ from the set, if there is no other point $k$ in the set such that the distance from $j$ to $k$ is <span class="tex-font-style-bf">strictly less</span> than the distance from $j$ to $i$. In other words, all other points from the set have distance to $j$ greater or equal to $|i - j|$.</p><p>For example, consider a set of points $\{1, 3, 5, 8\}$:</p><ul> <li> for the point $1$, the closest point is $3$ (other points have distance greater than $|1-3| = 2$); </li><li> for the point $3$, there are two closest points: $1$ and $5$; </li><li> for the point $5$, the closest point is $3$ (but not $8$, since its distance is greater than $|3-5|$); </li><li> for the point $8$, the closest point is $5$. </li></ul><p>You are given a set of points. You have to add an <span class="tex-font-style-bf">integer</span> point into this set in such a way that <span class="tex-font-style-bf">it is different from every existing point in the set</span>, and <span class="tex-font-style-bf">it becomes the closest point to every point in the set</span>. Is it possible?</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 1000$) ！ the number of test cases.</p><p>Each test case consists of two lines:</p><ul> <li> the first line contains one integer $n$ ($2 \le n \le 40$) ！ the number of points in the set; </li><li> the second line contains $n$ integers $x_1, x_2, \dots, x_n$ ($1 \le x_1 &lt; x_2 &lt; \dots &lt; x_n \le 100$) ！ the points from the set. </li></ul></div><div class="output-specification"><p>For each test case, print <span class="tex-font-style-tt">YES</span> if it is possible to add a new point according to the conditions from the statement. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 1000$) ！ the number of test cases.</p><p>Each test case consists of two lines:</p><ul> <li> the first line contains one integer $n$ ($2 \le n \le 40$) ！ the number of points in the set; </li><li> the second line contains $n$ integers $x_1, x_2, \dots, x_n$ ($1 \le x_1 &lt; x_2 &lt; \dots &lt; x_n \le 100$) ！ the points from the set. </li></ul>

## Output

<p>For each test case, print <span class="tex-font-style-tt">YES</span> if it is possible to add a new point according to the conditions from the statement. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p>





```input1|2,3,6,7
3
2
3 8
2
5 6
6
1 2 3 4 5 10
```




```output1
YES
NO
NO
```



## Note

<p>In the first example, the point $7$ will be the closest to both $3$ and $8$.</p><p>In the second example, it is impossible to add an <span class="tex-font-style-bf">integer</span> point so that it becomes the closest to both $5$ and $6$, and is different from both of them.</p>
