## Description

<div><div class="epigraph"><div class="epigraph-text"><a href="https://www.youtube.com/watch?v=55Ca6av1kAY"><span class="tex-font-style-it">Sakuzyo - Imprinting</span></a></div></div><p>A.R.C. Markland-N is a tall building with $n$ floors numbered from $1$ to $n$. Between each two adjacent floors in the building, there is a staircase connecting them.</p><p>It's lunchtime for our sensei Colin "ConneR" Neumann Jr, and he's planning for a location to enjoy his meal.</p><p>ConneR's office is at floor $s$ of the building. On each floor (including floor $s$, of course), there is a restaurant offering meals. However, due to renovations being in progress, $k$ of the restaurants are currently closed, and as a result, ConneR can't enjoy his lunch there.</p><p>CooneR wants to reach a restaurant as quickly as possible to save time. What is the minimum number of staircases he needs to walk to reach a closest currently open restaurant.</p><p>Please answer him quickly, and you might earn his praise and even enjoy the lunch with him in the elegant Neumanns' way!</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 1000$)&nbsp;！ the number of test cases in the test. Then the descriptions of $t$ test cases follow.</p><p>The first line of a test case contains three integers $n$, $s$ and $k$ ($2 \le n \le 10^9$, $1 \le s \le n$, $1 \le k \le \min(n-1, 1000)$)&nbsp;！ respectively the number of floors of A.R.C. Markland-N, the floor where ConneR is in, and the number of closed restaurants.</p><p>The second line of a test case contains $k$ distinct integers $a_1, a_2, \ldots, a_k$ ($1 \le a_i \le n$)&nbsp;！ the floor numbers of the currently closed restaurants.</p><p>It is guaranteed that the sum of $k$ over all test cases does not exceed $1000$.</p></div><div class="output-specification"><p>For each test case print a single integer&nbsp;！ the minimum number of staircases required for ConneR to walk from the floor $s$ to a floor with an open restaurant.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 1000$)&nbsp;！ the number of test cases in the test. Then the descriptions of $t$ test cases follow.</p><p>The first line of a test case contains three integers $n$, $s$ and $k$ ($2 \le n \le 10^9$, $1 \le s \le n$, $1 \le k \le \min(n-1, 1000)$)&nbsp;！ respectively the number of floors of A.R.C. Markland-N, the floor where ConneR is in, and the number of closed restaurants.</p><p>The second line of a test case contains $k$ distinct integers $a_1, a_2, \ldots, a_k$ ($1 \le a_i \le n$)&nbsp;！ the floor numbers of the currently closed restaurants.</p><p>It is guaranteed that the sum of $k$ over all test cases does not exceed $1000$.</p>

## Output

<p>For each test case print a single integer&nbsp;！ the minimum number of staircases required for ConneR to walk from the floor $s$ to a floor with an open restaurant.</p>

## Samples

```input1
5
5 2 3
1 2 3
4 3 3
4 1 2
10 2 6
1 2 3 4 5 7
2 1 1
2
100 76 8
76 75 36 67 41 74 10 77
```

```output1
2
0
4
0
2
```




## Note

<p>In the first example test case, the nearest floor with an open restaurant would be the floor $4$.</p><p>In the second example test case, the floor with ConneR's office still has an open restaurant, so Sensei won't have to go anywhere.</p><p>In the third example test case, the closest open restaurant is on the $6$-th floor.</p>
