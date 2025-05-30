## Description

<div><p><span class="tex-font-style-it">Captain Fint is involved in another treasure hunt, but have found only one strange problem. The problem may be connected to the treasure's location or may not. That's why captain Flint decided to leave the solving the problem to his crew and offered an absurdly high reward: one day off. The problem itself sounds like this...</span></p><p>There are two arrays $a$ and $b$ of length $n$. Initially, an $ans$ is equal to $0$ and the following operation is defined: </p><ol> <li> Choose position $i$ ($1 \le i \le n$); </li><li> Add $a_i$ to $ans$; </li><li> If $b_i \neq -1$ then add $a_i$ to $a_{b_i}$. </li></ol><p>What is the maximum $ans$ you can get by performing the operation on each $i$ ($1 \le i \le n$) <span class="tex-font-style-it">exactly once</span>?</p><p>Uncle Bogdan is eager to get the reward, so he is asking your help to find the optimal order of positions to perform the operation on them.</p></div><div class="input-specification"><p>The first line contains the integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the length of arrays $a$ and $b$.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($−10^6 \le a_i \le 10^6$).</p><p>The third line contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \le b_i \le n$ or $b_i = -1$).</p><p><span class="tex-font-style-bf">Additional constraint: it's guaranteed that for any $i$ ($1 \le i \le n$) the sequence $b_i, b_{b_i}, b_{b_{b_i}}, \ldots$ is not cyclic, in other words it will always end with $-1$.</span></p></div><div class="output-specification"><p>In the first line, print the maximum $ans$ you can get.</p><p>In the second line, print the order of operations: $n$ different integers $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le n$). The $p_i$ is the position which should be chosen at the $i$-th step. If there are multiple orders, print any of them.</p></div>

## Input

<p>The first line contains the integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the length of arrays $a$ and $b$.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($−10^6 \le a_i \le 10^6$).</p><p>The third line contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \le b_i \le n$ or $b_i = -1$).</p><p><span class="tex-font-style-bf">Additional constraint: it's guaranteed that for any $i$ ($1 \le i \le n$) the sequence $b_i, b_{b_i}, b_{b_{b_i}}, \ldots$ is not cyclic, in other words it will always end with $-1$.</span></p>

## Output

<p>In the first line, print the maximum $ans$ you can get.</p><p>In the second line, print the order of operations: $n$ different integers $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le n$). The $p_i$ is the position which should be chosen at the $i$-th step. If there are multiple orders, print any of them.</p>

## Samples

```input1
3
1 2 3
2 3 -1
```

```output1
10
1 2 3
```






```input2
2
-1 100
2 -1
```

```output2
99
2 1
```






```input3
10
-10 -1 2 2 5 -2 -3 -4 2 -6
-1 -1 2 2 -1 5 5 7 7 9
```

```output3
-9
3 5 6 1 9 4 10 7 8 2
```



