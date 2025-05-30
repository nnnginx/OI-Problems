## Description

<div><p>Polycarp calls an array dense if the greater of any two adjacent elements is not more than twice bigger than the smaller. More formally, for any $i$ ($1 \le i \le n-1$), this condition must be satisfied: $$\frac{\max(a[i], a[i+1])}{\min(a[i], a[i+1])} \le 2$$</p><p>For example, the arrays $[1, 2, 3, 4, 3]$, $[1, 1, 1]$ and $[5, 10]$ are dense. And the arrays $[5, 11]$, $[1, 4, 2]$, $[6, 6, 1]$ are <span class="tex-font-style-bf">not</span> dense.</p><p>You are given an array $a$ of $n$ integers. What is the minimum number of numbers you need to add to an array to make it dense? You can insert numbers anywhere in the array. If the array is already dense, no numbers need to be added.</p><p>For example, if $a=[4,2,10,1]$, then the answer is $5$, and the array itself after inserting elements into it may look like this: $a=[4,2,\underline{\textbf{3}},\underline{\textbf{5}},10,\underline{\textbf{6}},\underline{\textbf{4}},\underline{\textbf{2}},1]$ (there are other ways to build such $a$).</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 1000$). Then $t$ test cases follow.</p><p>The first line of each test case contains one integer $n$ ($2 \le n \le 50$)&nbsp;�� the length of the array $a$.</p><p>The next line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 50$).</p></div><div class="output-specification"><p>For each test case, output one integer&nbsp;�� the minimum number of numbers that must be added to the array to make it dense.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 1000$). Then $t$ test cases follow.</p><p>The first line of each test case contains one integer $n$ ($2 \le n \le 50$)&nbsp;�� the length of the array $a$.</p><p>The next line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 50$).</p>

## Output

<p>For each test case, output one integer&nbsp;�� the minimum number of numbers that must be added to the array to make it dense.</p>

## Samples

```input1
6
4
4 2 10 1
2
1 3
2
6 1
3
1 4 2
5
1 2 3 4 3
12
4 31 25 50 30 20 34 46 42 16 15 16
```

```output1
5
1
2
1
0
3
```




## Note

<p>The first test case is explained in the statements.</p><p>In the second test case, you can insert one element, $a=[1,\underline{\textbf{2}},3]$.</p><p>In the third test case, you can insert two elements, $a=[6,\underline{\textbf{4}},\underline{\textbf{2}},1]$.</p><p>In the fourth test case, you can insert one element, $a=[1,\underline{\textbf{2}},4,2]$.</p><p>In the fifth test case, the array $a$ is already dense.</p>
