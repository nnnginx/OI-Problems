## Description

<div><p>Let's say you are standing on the $XY$-plane at point $(0, 0)$ and you want to reach point $(n, n)$.</p><p>You can move only in two directions: </p><ul> <li> to the <span class="tex-font-style-it">right</span>, i.&nbsp;e. horizontally and in the direction that increase your $x$ coordinate, </li><li> or <span class="tex-font-style-it">up</span>, i.&nbsp;e. vertically and in the direction that increase your $y$ coordinate. </li></ul><p>In other words, your path will have the following structure: </p><ul> <li> initially, you choose to go to the right or up; </li><li> then you go some <span class="tex-font-style-bf">positive integer</span> distance in the chosen direction (distances can be chosen independently); </li><li> after that you change your direction (from right to up, or from up to right) and repeat the process. </li></ul><p>You don't like to change your direction too much, so you will make no more than $n - 1$ direction changes.</p><p>As a result, your path will be a polygonal chain from $(0, 0)$ to $(n, n)$, consisting of <span class="tex-font-style-bf">at most</span> $n$ line segments where each segment has positive integer length and vertical and horizontal segments alternate.</p><p>Not all paths are equal. You have $n$ integers $c_1, c_2, \dots, c_n$ where $c_i$ is the cost of the $i$-th segment.</p><p>Using these costs we can define the <span class="tex-font-style-it">cost of the path</span> as the sum of lengths of the segments of this path multiplied by their cost, i.&nbsp;e. if the path consists of $k$ segments ($k \le n$), then the cost of the path is equal to $\sum\limits_{i=1}^{k}{c_i \cdot length_i}$ (segments are numbered from $1$ to $k$ in the order they are in the path).</p><p>Find the path of the minimum cost and print its cost.</p></div><div class="input-specification"><p>The first line contains the single integer $t$ ($1 \le t \le 1000$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains the single integer $n$ ($2 \le n \le 10^5$).</p><p>The second line of each test case contains $n$ integers $c_1, c_2, \dots, c_n$ ($1 \le c_i \le 10^9$)&nbsp;！ the costs of each segment.</p><p>It's guaranteed that the total sum of $n$ doesn't exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print the minimum possible cost of the path from $(0, 0)$ to $(n, n)$ consisting of at most $n$ alternating segments.</p></div>

## Input

<p>The first line contains the single integer $t$ ($1 \le t \le 1000$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains the single integer $n$ ($2 \le n \le 10^5$).</p><p>The second line of each test case contains $n$ integers $c_1, c_2, \dots, c_n$ ($1 \le c_i \le 10^9$)&nbsp;！ the costs of each segment.</p><p>It's guaranteed that the total sum of $n$ doesn't exceed $10^5$.</p>

## Output

<p>For each test case, print the minimum possible cost of the path from $(0, 0)$ to $(n, n)$ consisting of at most $n$ alternating segments.</p>

## Samples

```input1
3
2
13 88
3
2 3 1
5
4 3 2 1 4
```

```output1
202
13
19
```




## Note

<p>In the first test case, to reach $(2, 2)$ you need to make at least one turn, so your path will consist of exactly $2$ segments: one horizontal of length $2$ and one vertical of length $2$. The cost of the path will be equal to $2 \cdot c_1 + 2 \cdot c_2 = 26 + 176 = 202$.</p><p>In the second test case, one of the optimal paths consists of $3$ segments: the first segment of length $1$, the second segment of length $3$ and the third segment of length $2$.</p><p>The cost of the path is $1 \cdot 2 + 3 \cdot 3 + 2 \cdot 1 = 13$.</p><p>In the third test case, one of the optimal paths consists of $4$ segments: the first segment of length $1$, the second one&nbsp;！ $1$, the third one&nbsp;！ $4$, the fourth one&nbsp;！ $4$. The cost of the path is $1 \cdot 4 + 1 \cdot 3 + 4 \cdot 2 + 4 \cdot 1 = 19$.</p>
