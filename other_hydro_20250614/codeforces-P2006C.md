## Description

<div><p>Let there be a set that contains <span class="tex-font-style-bf">distinct</span> positive integers. To expand the set to contain as many integers as possible, Eri can choose two integers $x\neq y$ from the set such that their average $\frac{x+y}2$ is still a positive integer and isn't contained in the set, and add it to the set. The integers $x$ and $y$ remain in the set.</p><p>Let's call the set of integers <span class="tex-font-style-it">consecutive</span> if, after the elements are sorted, the difference between any pair of adjacent elements is $1$. For example, sets $\{2\}$, $\{2, 5, 4, 3\}$, $\{5, 6, 8, 7\}$ are consecutive, while $\{2, 4, 5, 6\}$, $\{9, 7\}$ are not.</p><p>Eri likes consecutive sets. Suppose there is an array $b$, then Eri puts all elements in $b$ into the set. If after a finite number of operations described above, the set can become consecutive, the array $b$ will be called <span class="tex-font-style-it">brilliant</span>.</p><p>Note that if the same integer appears in the array multiple times, we only put it into the set <span class="tex-font-style-bf">once</span>, as a set always contains distinct positive integers.</p><p>Eri has an array $a$ of $n$ positive integers. Please help him to count the number of pairs of integers $(l,r)$ such that $1 \leq l \leq r \leq n$ and the subarray $a_l, a_{l+1}, \ldots, a_r$ is brilliant.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 4 \cdot 10^5$)&nbsp;！ length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots a_n$ ($1 \leq a_i \leq 10^9$)&nbsp;！ the elements of the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $4 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer ！ the number of brilliant subarrays.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 4 \cdot 10^5$)&nbsp;！ length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots a_n$ ($1 \leq a_i \leq 10^9$)&nbsp;！ the elements of the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $4 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer ！ the number of brilliant subarrays.</p>





```input1|2,3,6,7,10,11
6
2
2 2
6
1 3 6 10 15 21
5
6 30 18 36 9
1
1000000000
6
1 1 4 5 1 4
12
70 130 90 90 90 108 612 500 451 171 193 193
```




```output1
3
18
5
1
18
53
```



## Note

<p>In the first test case, the array $a = [2, 2]$ has $3$ subarrays: $[2]$, $[2]$, and $[2, 2]$. For all of them, the set only contains a single integer $2$, therefore it's always consecutive. All these subarrays are brilliant, so the answer is $3$.</p><p>In the second test case, let's consider the subarray $[3, 6, 10]$. We can do operations as follows:</p><center> $$\{3,6,10\} \xrightarrow{x=6,y=10} \{3,6,8,10\} \xrightarrow{x=6,y=8} \{3,6,7,8,10\} \xrightarrow{x=3,y=7} \{3,5,6,7,8,10\}$$   $$\xrightarrow{x=3,y=5} \{3,4,5,6,7,8,10\} \xrightarrow{x=8,y=10} \{3,4,5,6,7,8,9,10\}$$ </center><p>$\{3,4,5,6,7,8,9,10\}$ is a consecutive set, so the subarray $[3, 6, 10]$ is brilliant.</p>
