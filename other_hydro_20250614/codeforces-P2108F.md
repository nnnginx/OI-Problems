## Description

<div><p> </p><p>Pizano built an array $a$ of $n$ towers, each consisting of $a_i \ge 0$ blocks.</p><p>Pizano can knock down a tower so that the next $a_i$ towers grow by $1$. In other words, he can take the element $a_i$, increase the next $a_i$ elements by one, and then set $a_i$ to $0$. The blocks that fall outside the array of towers disappear. If Pizano knocks down a tower with $0$ blocks, nothing happens.</p><p>Pizano wants to knock down all $n$ towers in any order, <span class="tex-font-style-bf">each exactly once</span>. That is, for each $i$ from $1$ to $n$, he will knock down the tower at position $i$ exactly once.</p><p>Moreover, the resulting array of tower heights <span class="tex-font-style-bf">must be non-decreasing</span>. This means that after he knocks down all $n$ towers, for any $i &lt; j$, the tower at position $i$ must not be taller than the tower at position $j$.</p><p>You are required to output the maximum $\text{MEX}$ of the resulting array of tower heights.</p><p>The $\text{MEX}$ of an array is the smallest non-negative integer that is not present in the array.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 10^5$)&nbsp;！ the number of towers.</p><p>The second line of each test case contains $n$ integers&nbsp;！ the initial heights of the towers $a_1, \ldots, a_n$ ($0 \leq a_i \leq 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$. </p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the maximum $\text{MEX}$ of the final array.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 10^5$)&nbsp;！ the number of towers.</p><p>The second line of each test case contains $n$ integers&nbsp;！ the initial heights of the towers $a_1, \ldots, a_n$ ($0 \leq a_i \leq 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$. </p>

## Output

<p>For each test case, output a single integer&nbsp;！ the maximum $\text{MEX}$ of the final array.</p>





```input1|2,3,6,7,10,11,14,15
8
2
1 2
4
2 1 0 0
10
5 9 3 7 1 5 1 5 4 3
10
1 1 1 1 1 1 1 1 1 1
10
3 2 1 0 3 2 1 0 3 2
5
5 2 0 5 5
1
1000000000
7
4 0 1 0 2 7 7
```




```output1
2
3
7
4
5
4
1
3
```



## Note

<p>Explanation for the first test case. </p><center>  <img class="tex-graphics" src="./37116/file/0QVgYlzx.png" style="max-width: 100.0%;max-height: 100.0%;" width="450px"> </center><p>Explanation for the second test case. Note that all towers were knocked down exactly once, and the final array of heights is non-decreasing. </p><center>  <img class="tex-graphics" src="./37116/file/cGhLkml2.png" style="max-width: 100.0%;max-height: 100.0%;" width="675px"> </center>
