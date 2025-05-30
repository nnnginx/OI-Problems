## Description

<div><p>Polycarp found on the street an array $a$ of $n$ elements.</p><p>Polycarp invented his criterion for the beauty of an array. He calls an array $a$ beautiful if at least one of the following conditions must be met <span class="tex-font-style-bf">for each different pair of indices</span> $i \ne j$: </p><ul> <li> $a_i$ is divisible by $a_j$; </li><li> or $a_j$ is divisible by $a_i$. </li></ul><p>For example, if: </p><ul> <li> $n=5$ and $a=[7, 9, 3, 14, 63]$, then the $a$ array is not beautiful (for $i=4$ and $j=2$, none of the conditions above is met); </li><li> $n=3$ and $a=[2, 14, 42]$, then the $a$ array is beautiful; </li><li> $n=4$ and $a=[45, 9, 3, 18]$, then the $a$ array is not beautiful (for $i=1$ and $j=4$ none of the conditions above is met); </li></ul><p>Ugly arrays upset Polycarp, so he wants to remove some elements from the array $a$ so that it becomes beautiful. Help Polycarp determine the smallest number of elements to remove to make the array $a$ beautiful.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \leq t \leq 10$)&nbsp;！ the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case contains one integer $n$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;！ the length of the array $a$.</p><p>The second line of each test case contains $n$ numbers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 2 \cdot 10^5$)&nbsp;！ elements of the array $a$.</p></div><div class="output-specification"><p>For each test case output one integer&nbsp;！ the minimum number of elements that must be removed to make the array $a$ beautiful.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \leq t \leq 10$)&nbsp;！ the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case contains one integer $n$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;！ the length of the array $a$.</p><p>The second line of each test case contains $n$ numbers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 2 \cdot 10^5$)&nbsp;！ elements of the array $a$.</p>

## Output

<p>For each test case output one integer&nbsp;！ the minimum number of elements that must be removed to make the array $a$ beautiful.</p>

## Samples

```input1
4
5
7 9 3 14 63
3
2 14 42
4
45 9 3 18
3
2 2 8
```

```output1
2
0
1
0
```




## Note

<p>In the first test case, removing $7$ and $14$ will make array $a$ beautiful.</p><p>In the second test case, the array $a$ is already beautiful.</p><p>In the third test case, removing one of the elements $45$ or $18$ will make the array $a$ beautiful.</p><p>In the fourth test case, the array $a$ is beautiful.</p>
