## Description

<div><p>Dark is going to attend Motarack's birthday. Dark decided that the gift he is going to give to Motarack is an array $a$ of $n$ non-negative integers.</p><p>Dark created that array $1000$ years ago, so some elements in that array disappeared. Dark knows that Motarack hates to see an array that has two adjacent elements with a high absolute difference between them. He doesn't have much time so he wants to choose an integer $k$ ($0 \leq k \leq 10^{9}$) and replaces all missing elements in the array $a$ with $k$.</p><p>Let $m$ be the maximum absolute difference between all adjacent elements (i.e. the maximum value of $|a_i - a_{i+1}|$ for all $1 \leq i \leq n - 1$) in the array $a$ after Dark replaces all missing elements with $k$.</p><p>Dark should choose an integer $k$ so that $m$ is minimized. Can you help him?</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) &nbsp;�� the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains one integer $n$ ($2 \leq n \leq 10^{5}$)&nbsp;�� the size of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-1 \leq a_i \leq 10 ^ {9}$). If $a_i = -1$, then the $i$-th integer is missing. It is guaranteed that at least one integer is missing in every test case.</p><p>It is guaranteed, that the sum of $n$ for all test cases does not exceed $4 \cdot 10 ^ {5}$.</p></div><div class="output-specification"><p>Print the answers for each test case in the following format:</p><p>You should print two integers, the minimum possible value of $m$ and an integer $k$ ($0 \leq k \leq 10^{9}$) that makes the maximum absolute difference between adjacent elements in the array $a$ equal to $m$.</p><p>Make sure that after replacing all the missing elements with $k$, the maximum absolute difference between adjacent elements becomes $m$.</p><p>If there is more than one possible $k$, you can print any of them.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) &nbsp;�� the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains one integer $n$ ($2 \leq n \leq 10^{5}$)&nbsp;�� the size of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-1 \leq a_i \leq 10 ^ {9}$). If $a_i = -1$, then the $i$-th integer is missing. It is guaranteed that at least one integer is missing in every test case.</p><p>It is guaranteed, that the sum of $n$ for all test cases does not exceed $4 \cdot 10 ^ {5}$.</p>

## Output

<p>Print the answers for each test case in the following format:</p><p>You should print two integers, the minimum possible value of $m$ and an integer $k$ ($0 \leq k \leq 10^{9}$) that makes the maximum absolute difference between adjacent elements in the array $a$ equal to $m$.</p><p>Make sure that after replacing all the missing elements with $k$, the maximum absolute difference between adjacent elements becomes $m$.</p><p>If there is more than one possible $k$, you can print any of them.</p>

## Samples

```input1
7
5
-1 10 -1 12 -1
5
-1 40 35 -1 35
6
-1 -1 9 -1 3 -1
2
-1 -1
2
0 -1
4
1 -1 3 -1
7
1 -1 7 5 2 -1 5
```

```output1
1 11
5 35
3 6
0 42
0 0
1 2
3 4
```




## Note

<p>In the first test case after replacing all missing elements with $11$ the array becomes $[11, 10, 11, 12, 11]$. The absolute difference between any adjacent elements is $1$. It is impossible to choose a value of $k$, such that the absolute difference between any adjacent element will be $\leq 0$. So, the answer is $1$.</p><p>In the third test case after replacing all missing elements with $6$ the array becomes $[6, 6, 9, 6, 3, 6]$.</p><ul> <li> $|a_1 - a_2| = |6 - 6| = 0$; </li><li> $|a_2 - a_3| = |6 - 9| = 3$; </li><li> $|a_3 - a_4| = |9 - 6| = 3$; </li><li> $|a_4 - a_5| = |6 - 3| = 3$; </li><li> $|a_5 - a_6| = |3 - 6| = 3$. </li></ul><p>So, the maximum difference between any adjacent elements is $3$.</p>
