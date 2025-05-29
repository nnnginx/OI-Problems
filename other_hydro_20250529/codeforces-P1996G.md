## Description

<div><p>On <span class="tex-font-style-it">Penacony, The Land of the Dreams</span>, there exists $n$ houses and $n$ roads. There exists a road between house $i$ and $i+1$ for all $1 \leq i \leq n-1$ and a road between house $n$ and house $1$. All roads are bidirectional. However, due to the crisis on Penacony, the overseeing family has gone into debt and may not be able to maintain all roads.</p><p>There are $m$ pairs of friendships between the residents of Penacony. If the resident living in house $a$ is friends with the resident living in house $b$, there must be a path between houses $a$ and $b$ through maintained roads. </p><p>What is the minimum number of roads that must be maintained?</p></div><div class="input-specification"><p>The first line contains $t$ ($1 \leq t \leq 10^4$) 每 the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($3 \leq n \leq 2 \cdot 10^5, 1 \leq m \leq 2 \cdot 10^5$) 每 the number of houses and the number of friendships.</p><p>The next $m$ lines contain two integers $a$ and $b$ ($1 \leq a &lt; b \leq n$) 每 the resident in house $a$ is friends with the resident in house $b$. It is guaranteed all ($a, b$) are distinct.</p><p>It is guaranteed the sum of $n$ and $m$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output an integer, the minimum number of roads that must be maintained.</p></div>

## Input

<p>The first line contains $t$ ($1 \leq t \leq 10^4$) 每 the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($3 \leq n \leq 2 \cdot 10^5, 1 \leq m \leq 2 \cdot 10^5$) 每 the number of houses and the number of friendships.</p><p>The next $m$ lines contain two integers $a$ and $b$ ($1 \leq a &lt; b \leq n$) 每 the resident in house $a$ is friends with the resident in house $b$. It is guaranteed all ($a, b$) are distinct.</p><p>It is guaranteed the sum of $n$ and $m$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output an integer, the minimum number of roads that must be maintained.</p>





```input1|2,3,4,5,11,12,13,19,20,24,25,26
7
8 3
1 8
2 7
4 5
13 4
1 13
2 12
3 11
4 10
10 2
2 3
3 4
10 4
3 8
5 10
2 10
4 10
4 1
1 3
5 2
3 5
1 4
5 2
2 5
1 3
```




```output1
4
7
2
7
2
3
3
```



## Note

<p>For the first test case, the following roads must be maintained:</p><ul> <li> $8 \leftarrow \rightarrow 1$ </li><li> $7 \leftarrow \rightarrow 8$ </li><li> $1 \leftarrow \rightarrow 2$ </li><li> $4 \leftarrow \rightarrow 5$ </li></ul>
