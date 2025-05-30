## Description

<div><p>Alexander is a well-known programmer. Today he decided to finally go out and play football, but with the first hit he left a dent on the new Rolls-Royce of the wealthy businessman Big Vova. Vladimir has recently opened a store on the popular online marketplace "Zmey-Gorynych", and offers Alex a job: if he shows his programming skills by solving a task, he'll work as a cybersecurity specialist. Otherwise, he'll be delivering some doubtful products for the next two years.</p><p>You're given $n$ positive integers $a_1, a_2, \dots, a_n$. Using each of them <span class="tex-font-style-bf">exactly at once</span>, you're to make such sequence $b_1, b_2, \dots, b_n$ that sequence $c_1, c_2, \dots, c_n$ is <span class="tex-font-style-it">lexicographically maximal</span>, where $c_i=GCD(b_1,\dots,b_i)$ - the greatest common divisor of the first $i$ elements of $b$. </p><p>Alexander is really afraid of the conditions of this simple task, so he asks you to solve it.</p><p>A sequence $a$ is lexicographically smaller than a sequence $b$ if and only if one of the following holds:</p><ul><li> $a$ is a prefix of $b$, but $a \ne b$;</li><li> in the first position where $a$ and $b$ differ, the sequence $a$ has a smaller element than the corresponding element in $b$.</li></ul></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^3$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^3$) &nbsp;！ the length of the sequence $a$.</p><p>The second line of each test case contains $n$ integers $a_1,\dots,a_n$ ($1 \le a_i \le 10^3$) &nbsp;！ the sequence $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^3$.</p></div><div class="output-specification"><p>For each test case output the answer in a single line &nbsp;！ the desired sequence $b$. If there are multiple answers, print any.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^3$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^3$) &nbsp;！ the length of the sequence $a$.</p><p>The second line of each test case contains $n$ integers $a_1,\dots,a_n$ ($1 \le a_i \le 10^3$) &nbsp;！ the sequence $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^3$.</p>

## Output

<p>For each test case output the answer in a single line &nbsp;！ the desired sequence $b$. If there are multiple answers, print any.</p>

## Samples

```input1
7
2
2 5
4
1 8 2 3
3
3 8 9
5
64 25 75 100 50
1
42
6
96 128 88 80 52 7
5
2 4 8 16 17
```

```output1
5 2 
8 2 1 3 
9 3 8 
100 50 25 75 64 
42 
128 96 80 88 52 7 
17 2 4 8 16
```




## Note

<p>In the first test case of the example, there are only two possible permutations $b$ &nbsp;！ $[2, 5]$ and $[5, 2]$: for the first one $c=[2, 1]$, for the second one $c=[5, 1]$.</p><p>In the third test case of the example, number $9$ should be the first in $b$, and $GCD(9, 3)=3$, $GCD(9, 8)=1$, so the second number of $b$ should be $3$.</p><p>In the seventh test case of the example, first four numbers pairwise have a common divisor (a power of two), but none of them can be the first in the optimal permutation $b$.</p>
