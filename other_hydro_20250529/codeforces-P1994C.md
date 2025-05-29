## Description

<div><p>Yaroslav is playing a computer game, and at one of the levels, he encountered $n$ mushrooms arranged in a row. Each mushroom has its own level of toxicity; the $i$-th mushroom from the beginning has a toxicity level of $a_i$. Yaroslav can choose two integers $1 \le l \le r \le n$, and then his character will take turns from left to right to eat mushrooms from this subsegment one by one, i.e., the mushrooms with numbers $l, l+1, l+2, \ldots, r$.</p><p>The character has a toxicity level $g$, initially equal to $0$. The computer game is defined by the number $x$&nbsp;！ the maximum toxicity level at any given time. When eating a mushroom with toxicity level $k$, the following happens:</p><ol> <li> The toxicity level of the character is increased by $k$. </li><li> If $g \leq x$, the process continues; otherwise, $g$ becomes zero and the process continues. </li></ol><p>Yaroslav became interested in how many ways there are to choose the values of $l$ and $r$ such that the final value of $g$ is not zero. Help Yaroslav find this number!</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains an integer $t$ ($1 \le t \le 10^{4}$)&nbsp;！ the number of test cases. Then follows the description of the test cases.</p><p>The first line of each test case contains two integers $n$, $x$ ($1 \leq n \leq 2 \cdot 10^5, 1 \le x \le 10^9$)&nbsp;！ the number of mushrooms and the maximum toxicity level.</p><p>The second line of each test case contains $n$ numbers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single number&nbsp;！ the number of subsegments such that the final value of $g$ will not be zero.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains an integer $t$ ($1 \le t \le 10^{4}$)&nbsp;！ the number of test cases. Then follows the description of the test cases.</p><p>The first line of each test case contains two integers $n$, $x$ ($1 \leq n \leq 2 \cdot 10^5, 1 \le x \le 10^9$)&nbsp;！ the number of mushrooms and the maximum toxicity level.</p><p>The second line of each test case contains $n$ numbers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single number&nbsp;！ the number of subsegments such that the final value of $g$ will not be zero.</p>





```input1|2,3,6,7,10,11
5
4 2
1 1 1 1
3 2
1 2 3
1 6
10
6 3
1 2 1 4 3 8
5 999999999
999999999 999999998 1000000000 1000000000 500000000
```




```output1
8
2
0
10
7
```



## Note

<p>In the first test case, the subsegments $(1, 1)$, $(1, 2)$, $(1, 4)$, $(2, 2)$, $(2, 3)$, $(3, 3)$, $(3, 4)$ and $(4, 4)$ are suitable.</p><p>In the second test case, non-zero $g$ will remain only on the subsegments $(1, 1)$ and $(2, 2)$.</p><p>In the third test case, on the only possible subsegment, $g$ will be zero.</p>
