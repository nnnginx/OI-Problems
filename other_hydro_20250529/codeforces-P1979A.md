## Description

<div><p>Alice and Bob came up with a rather strange game. They have an array of integers $a_1, a_2,\ldots, a_n$. Alice chooses a certain integer $k$ and tells it to Bob, then the following happens:</p><ul> <li> Bob chooses two integers $i$ and $j$ ($1 \le i &lt; j \le n$), and then finds the maximum among the integers $a_i, a_{i + 1},\ldots, a_j$; </li><li> If the obtained maximum is <span class="tex-font-style-bf">strictly greater</span> than $k$, Alice wins, otherwise Bob wins. </li></ul><p>Help Alice find the maximum $k$ at which she is guaranteed to win.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 5 \cdot 10^4$)&nbsp;！ the number of elements in the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2,\ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;！ the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5 \cdot 10^4$.</p></div><div class="output-specification"><p>For each test case, output one integer ！ the maximum integer $k$ at which Alice is guaranteed to win.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 5 \cdot 10^4$)&nbsp;！ the number of elements in the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2,\ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;！ the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5 \cdot 10^4$.</p>

## Output

<p>For each test case, output one integer ！ the maximum integer $k$ at which Alice is guaranteed to win.</p>





```input1|2,3,6,7,10,11
6
4
2 4 1 7
5
1 2 3 4 5
2
1 1
3
37 8 16
5
10 10 10 10 9
10
3 12 9 5 2 3 2 9 8 2
```




```output1
3
1
0
15
9
2
```



## Note

<p>In the first test case, all possible subsegments that Bob can choose look as follows: $[2, 4], [2, 4, 1], [2, 4, 1, 7], [4, 1], [4, 1, 7], [1, 7]$. The maximums on the subsegments are respectively equal to $4, 4, 7, 4, 7, 7$. It can be shown that $3$ is the largest integer such that any of the maximums will be strictly greater than it.</p><p>In the third test case, the only segment that Bob can choose is $[1, 1]$. So the answer is $0$.</p>
