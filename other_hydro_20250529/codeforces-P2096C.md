## Description

<div><p>You are the proud leader of a city in Ancient Berland. There are $n^2$ buildings arranged in a grid of $n$ rows and $n$ columns. The height of the building in row $i$ and column $j$ is $h_{i, j}$.</p><p>The city is <span class="tex-font-style-it">beautiful</span> if no two adjacent by side buildings have the same height. In other words, it must satisfy the following:</p><ul> <li> There <span class="tex-font-style-bf">does not</span> exist a position $(i, j)$ ($1 \leq i \leq n$, $1 \leq j \leq n - 1$) such that $h_{i, j} = h_{i, j + 1}$. </li><li> There <span class="tex-font-style-bf">does not</span> exist a position $(i, j)$ ($1 \leq i \leq n - 1$, $1 \leq j \leq n$) such that $h_{i, j} = h_{i + 1, j}$. </li></ul><p>There are $n$ workers at company A, and $n$ workers at company B. Each worker can be hired <span class="tex-font-style-bf">at most once</span>.</p><p>It costs $a_i$ coins to hire worker $i$ at company A. After hiring, worker $i$ will:</p><ul> <li> Increase the heights of all buildings in row $i$ by $1$. In other words, increase $h_{i, 1}, h_{i, 2}, \ldots, h_{i, n}$ by $1$. </li></ul><p>It costs $b_j$ coins to hire worker $j$ at company B. After hiring, worker $j$ will:</p><ul> <li> Increase the heights of all buildings in column $j$ by $1$. In other words, increase $h_{1, j}, h_{2, j}, \ldots, h_{n, j}$ by $1$. </li></ul><p>Find the minimum number of coins needed to make the city beautiful, or report that it is impossible.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 1000$)&nbsp;！ the size of the grid.</p><p>The $i$-th of the next $n$ lines of each test case contains $n$ integers $h_{i, 1}, h_{i, 2}, \ldots, h_{i, n}$ ($1 \le h_{i, j} \le 10^9$)&nbsp;！ the heights of the buildings in row $i$.</p><p>The next line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;！ the costs of hiring the workers at company A.</p><p>The next line of each test case contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \le b_j \le 10^9$)&nbsp;！ the costs of hiring the workers at company B.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $1000$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the minimum number of coins needed, or $-1$ if it is impossible.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 1000$)&nbsp;！ the size of the grid.</p><p>The $i$-th of the next $n$ lines of each test case contains $n$ integers $h_{i, 1}, h_{i, 2}, \ldots, h_{i, n}$ ($1 \le h_{i, j} \le 10^9$)&nbsp;！ the heights of the buildings in row $i$.</p><p>The next line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;！ the costs of hiring the workers at company A.</p><p>The next line of each test case contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \le b_j \le 10^9$)&nbsp;！ the costs of hiring the workers at company B.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $1000$.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the minimum number of coins needed, or $-1$ if it is impossible.</p>





```input1|2,3,4,5,6,14,15,16,17,18,19
4
2
1 2
2 1
100 100
100 100
4
1 2 1 2
3 2 1 2
1 2 1 1
1 3 1 2
1 2 3 4
5 6 7 8
3
1 2 2
2 2 1
2 1 1
100 100 100
100 100 100
6
8 7 2 8 4 8
7 7 9 7 1 1
8 3 1 1 8 5
6 8 3 1 1 4
1 4 5 1 9 6
7 1 1 6 8 2
11 23 20 79 30 15
15 83 73 57 34 63
```




```output1
0
14
-1
183
```



## Note

<p>For the first test case, we can see that the city is already beautiful. Thus, the answer is $0$.</p><p>For the second test case, we can hire worker $2$ from company A, worker $4$ from company A, and worker $4$ from company B:</p><center><p></p><table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$2$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\color{red}2$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right" rowspan="4">$\implies$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$2$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\color{red}3$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\color{red}3$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\color{red}2$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\color{red}1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\color{red}2$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\color{red}4$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\color{red}3$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\color{red}2$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\color{red}4$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$2$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\color{red}1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$2$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\color{red}2$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\color{red}1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\color{red}3$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\color{red}1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\color{red}2$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\color{red}2$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\color{red}4$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\color{red}2$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\color{red}4$</td></tr></tbody></table><p></p></center><p>The cost of hiring the workers is $2 + 4 + 8 = 14$. This is the minimum possible cost.</p><p>For the third test case, no matter what we do, it is impossible to make the city beautiful. Thus, the answer is $-1$. </p>
