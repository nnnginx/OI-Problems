## Description

<div><p>There are $100$ rooms arranged in a row and $99$ doors between them; the $i$-th door connects rooms $i$ and $i+1$. Each door can be either locked or unlocked. Initially, all doors are unlocked.</p><p>We say that room $x$ is reachable from room $y$ if all doors between them are unlocked.</p><p>You know that: </p><ul> <li> Alice is in some room from the segment $[l, r]$; </li><li> Bob is in some room from the segment $[L, R]$; </li><li> Alice and Bob are in different rooms. </li></ul><p>However, you don't know the exact rooms they are in.</p><p>You don't want Alice and Bob to be able to reach each other, so you are going to lock some doors to prevent that. What's the smallest number of doors you have to lock so that Alice and Bob cannot meet, regardless of their starting positions inside the given segments?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;�� the number of test cases.</p><p>The first line of each test case contains two integers $l$ and $r$ ($1 \le l &lt; r \le 100$)&nbsp;�� the bounds of the segment of rooms where Alice is located.</p><p>The second line of each test case contains two integers $L$ and $R$ ($1 \le L &lt; R \le 100$) �� the bounds of the segment of rooms where Bob is located.</p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;�� the smallest number of doors you have to lock so that Alice and Bob cannot meet, regardless of their starting positions inside the given segments.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;�� the number of test cases.</p><p>The first line of each test case contains two integers $l$ and $r$ ($1 \le l &lt; r \le 100$)&nbsp;�� the bounds of the segment of rooms where Alice is located.</p><p>The second line of each test case contains two integers $L$ and $R$ ($1 \le L &lt; R \le 100$) �� the bounds of the segment of rooms where Bob is located.</p>

## Output

<p>For each test case, print a single integer&nbsp;�� the smallest number of doors you have to lock so that Alice and Bob cannot meet, regardless of their starting positions inside the given segments.</p>





```input1|2,3,6,7
4
1 2
3 4
2 5
2 5
3 7
6 7
4 5
2 8
```




```output1
1
3
2
3
```



## Note

<p>In the first test case, it is sufficient to lock the door between rooms $2$ and $3$.</p><p>In the second test case, the following doors have to be locked: $(2,3)$, $(3,4)$, $(4,5)$.</p><p>In the third test case, the following doors have to be locked: $(5, 6)$ and $(6,7)$.</p>
