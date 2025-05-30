## Description

<div><p>Polycarp has $n$ friends, the $i$-th of his friends has $a_i$ candies. Polycarp's friends do not like when they have different numbers of candies. In other words they want all $a_i$ to be the same. To solve this, Polycarp performs the following set of actions exactly <span class="tex-font-style-bf">once</span>: </p><ul> <li> Polycarp chooses $k$ ($0 \le k \le n$) arbitrary friends (let's say he chooses friends with indices $i_1, i_2, \ldots, i_k$); </li><li> Polycarp distributes their $a_{i_1} + a_{i_2} + \ldots + a_{i_k}$ candies among all $n$ friends. During distribution for each of $a_{i_1} + a_{i_2} + \ldots + a_{i_k}$ candies he chooses new owner. That can be any of $n$ friends. Note, that any candy can be given to the person, who has owned that candy before the distribution process. </li></ul><p>Note that the number $k$ is not fixed in advance and can be arbitrary. Your task is to find the minimum value of $k$.</p><p>For example, if $n=4$ and $a=[4, 5, 2, 5]$, then Polycarp could make the following distribution of the candies: </p><ul> <li> Polycarp chooses $k=2$ friends with indices $i=[2, 4]$ and distributes $a_2 + a_4 = 10$ candies to make $a=[4, 4, 4, 4]$ (two candies go to person $3$). </li></ul><p>Note that in this example Polycarp cannot choose $k=1$ friend so that he can redistribute candies so that in the end all $a_i$ are equal.</p><p>For the data $n$ and $a$, determine the <span class="tex-font-style-bf">minimum</span> value $k$. With this value $k$, Polycarp should be able to select $k$ friends and redistribute their candies so that everyone will end up with the same number of candies.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$). Then $t$ test cases follow.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^4$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case output: </p><ul> <li> the minimum value of $k$, such that Polycarp can choose exactly $k$ friends so that he can redistribute the candies in the desired way; </li><li> "<span class="tex-font-style-tt">-1</span>" if no such value $k$ exists. </li></ul></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$). Then $t$ test cases follow.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^4$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case output: </p><ul> <li> the minimum value of $k$, such that Polycarp can choose exactly $k$ friends so that he can redistribute the candies in the desired way; </li><li> "<span class="tex-font-style-tt">-1</span>" if no such value $k$ exists. </li></ul>

## Samples

```input1
5
4
4 5 2 5
2
0 4
5
10 8 5 1 4
1
10000
7
1 1 1 1 1 1 1
```

```output1
2
1
-1
0
0
```



