## Description

<div><p> </p><center><table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-center tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-size-small"><span class="tex-font-style-it">On the next new moon, the universe will reset, beginning with Florida. It's up to Florida Man to stop it, but he first needs to find an important item.</span></span></td></tr></tbody></table></center><p>There are $n$ haystacks labelled from $1$ to $n$, where haystack $i$ contains $a_i$ haybales. One of the haystacks has a needle hidden beneath it, but you do not know which one. Your task is to move the haybales so that each haystack is emptied at least once, allowing you to check if the needle is hidden under that particular haystack.</p><p>However, the process is not that simple. Once a haystack $i$ is emptied for the first time, it will be assigned a height limit and can no longer contain more than $b_i$ haybales. More formally, a move is described as follows:</p><ul> <li> Choose two haystacks $i$ and $j$. If haystack $i$ has not been emptied before, or haystack $i$ contains strictly less than $b_i$ haybales, you may move exactly $1$ haybale from haystack $j$ to haystack $i$. </li></ul><p><span class="tex-font-style-bf">Note</span>: Before a haystack is emptied, it has no height limit, and you can move as many haybales as you want onto that haystack.</p><p>Compute the minimum number of moves required to ensure that each haystack is emptied at least once, or report that it is impossible.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($2\le n\le 5\cdot 10^5$)&nbsp;！ the number of haystacks.</p><p>The $i$-th of the next $n$ lines contains two integers $a_i$ and $b_i$ ($1\le a_i, b_i\le 10^9$)&nbsp;！ the initial number of haybales in the $i$-th haystack, and the height limit that it is assigned after it is emptied for the first time.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5 \cdot 10^5$. </p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;！ the minimum number of moves required to ensure that each haystack is emptied at least once. If it is not possible to empty each haystack at least once, output <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($2\le n\le 5\cdot 10^5$)&nbsp;！ the number of haystacks.</p><p>The $i$-th of the next $n$ lines contains two integers $a_i$ and $b_i$ ($1\le a_i, b_i\le 10^9$)&nbsp;！ the initial number of haybales in the $i$-th haystack, and the height limit that it is assigned after it is emptied for the first time.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5 \cdot 10^5$. </p>

## Output

<p>For each test case, print a single integer&nbsp;！ the minimum number of moves required to ensure that each haystack is emptied at least once. If it is not possible to empty each haystack at least once, output <span class="tex-font-style-tt">-1</span>.</p>





```input1|2,3,4,8,9,10,11,16,17,18,19,20,21,22,29,30,31
7
2
3 5
2 4
2
10 1
1 10
3
1 3
4 3
1 1
3
5 4
2 4
1 10
6
2 1
3 3
5 4
1 5
1 6
1 8
5
3 2
1 2
1 1
1 3
6 5
2
5 10
7 12
```




```output1
8
-1
8
9
14
15
19
```



## Note

<p>In the first test case, we can do the following sequence of moves:</p><ul> <li> Move $3$ haybales from haystack $1$ to haystack $2$. Haystack $1$ is now emptied, and is assigned a height limit of $5$. </li><li> Move $5$ haybales from haystack $2$ to haystack $1$. Haystack $2$ is now emptied, and is assigned a height limit of $4$. </li></ul><p>The above sequence requires $3 + 5 = 8$ moves. It is not possible to use less than $8$ moves as the following sequence of moves is invalid:</p><ul> <li> Move $2$ haybales from haystack $2$ to haystack $1$. Haystack $2$ is now emptied, and is assigned a height limit of $4$. </li><li> Move $4$ haybales from haystack $1$ to haystack $2$. Haystack $1$ now has $1$ haybale, while haystack $2$ has $4$ haybales. </li><li> Haystack $1$ cannot be emptied as haystack $2$ is already at its height limit of $4$, so no more haybales can be moved from haystack $1$ to haystack $2$. </li></ul><p>In the second test case, the task is impossible. This is because the height limits of both haystacks are too small that once one of the haystacks is emptied, the other haystack cannot be emptied due to the small height limits.</p><p>In the third test case, the following sequence of moves can be shown to be optimal:</p><ul> <li> Move $1$ haybale from haystack $1$ to haystack $3$. Haystack $1$ is now emptied, and is assigned a height limit of $3$. </li><li> Move $3$ haybales from haystack $2$ to haystack $1$. </li><li> Move $1$ haybale from haystack $2$ to haystack $3$. Haystack $2$ is now emptied and is assigned a height limit of $3$. </li><li> Move $3$ haybales from haystack $3$ to haystack $2$. Haystack $3$ is now emptied, and is assigned a height limit of $1$. </li></ul><p>The above sequence requires $1 + 3 + 1 + 3 = 8$ moves.</p>
