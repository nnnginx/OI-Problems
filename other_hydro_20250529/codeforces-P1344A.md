## Description

<div><p>Hilbert's Hotel is a very unusual hotel since the number of rooms is infinite! In fact, there is exactly one room for every integer, <span class="tex-font-style-bf">including zero and negative integers</span>. Even stranger, the hotel is currently at full capacity, meaning there is exactly one guest in every room. The hotel's manager, David Hilbert himself, decides he wants to shuffle the guests around because he thinks this will create a vacancy (a room without a guest).</p><p>For any integer $k$ and positive integer $n$, let $k\bmod n$ denote the remainder when $k$ is divided by $n$. More formally, $r=k\bmod n$ is the smallest non-negative integer such that $k-r$ is divisible by $n$. It always holds that $0\le k\bmod n\le n-1$. For example, $100\bmod 12=4$ and $(-1337)\bmod 3=1$.</p><p>Then the shuffling works as follows. There is an array of $n$ integers $a_0,a_1,\ldots,a_{n-1}$. Then for each integer $k$, the guest in room $k$ is moved to room number $k+a_{k\bmod n}$.</p><p>After this shuffling process, determine if there is still exactly one guest assigned to each room. That is, there are no vacancies or rooms with multiple guests.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1\le t\le 10^4$)&nbsp;�� the number of test cases. Next $2t$ lines contain descriptions of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1\le n\le 2\cdot 10^5$)&nbsp;�� the length of the array.</p><p>The second line of each test case contains $n$ integers $a_0,a_1,\ldots,a_{n-1}$ ($-10^9\le a_i\le 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single line containing "<span class="tex-font-style-tt">YES</span>" if there is exactly one guest assigned to each room after the shuffling process, or "<span class="tex-font-style-tt">NO</span>" otherwise. You can print each letter in any case (upper or lower).</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1\le t\le 10^4$)&nbsp;�� the number of test cases. Next $2t$ lines contain descriptions of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1\le n\le 2\cdot 10^5$)&nbsp;�� the length of the array.</p><p>The second line of each test case contains $n$ integers $a_0,a_1,\ldots,a_{n-1}$ ($-10^9\le a_i\le 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p>

## Output

<p>For each test case, output a single line containing "<span class="tex-font-style-tt">YES</span>" if there is exactly one guest assigned to each room after the shuffling process, or "<span class="tex-font-style-tt">NO</span>" otherwise. You can print each letter in any case (upper or lower).</p>

## Samples

```input1
6
1
14
2
1 -1
4
5 5 5 1
3
3 2 1
2
0 1
5
-239 -2 -100 -3 -11
```

```output1
YES
YES
YES
NO
NO
YES
```




## Note

<p>In the first test case, every guest is shifted by $14$ rooms, so the assignment is still unique.</p><p>In the second test case, even guests move to the right by $1$ room, and odd guests move to the left by $1$ room. We can show that the assignment is still unique.</p><p>In the third test case, every fourth guest moves to the right by $1$ room, and the other guests move to the right by $5$ rooms. We can show that the assignment is still unique.</p><p>In the fourth test case, guests $0$ and $1$ are both assigned to room $3$.</p><p>In the fifth test case, guests $1$ and $2$ are both assigned to room $2$.</p>
