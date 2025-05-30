## Description

<div><p>You are given an array $a$ consisting of $n$ integers.</p><p>In one move, you can choose some index $i$ ($1 \le i \le n - 2$) and shift the segment $[a_i, a_{i + 1}, a_{i + 2}]$ cyclically to the right (i.e. replace the segment $[a_i, a_{i + 1}, a_{i + 2}]$ with $[a_{i + 2}, a_i, a_{i + 1}]$). </p><p>Your task is to sort the initial array by <span class="tex-font-style-bf">no more than $n^2$ such operations</span> or say that it is impossible to do that.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 100$) �� the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($3 \le n \le 500$) �� the length of $a$. The second line of the test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 500$), where $a_i$ is the $i$-th element $a$.</p><p>It is guaranteed that the sum of $n$ does not exceed $500$.</p></div><div class="output-specification"><p>For each test case, print the answer: <span class="tex-font-style-tt">-1</span> on the only line if it is impossible to sort the given array using operations described in the problem statement, or the number of operations $ans$ on the first line and $ans$ integers $idx_1, idx_2, \dots, idx_{ans}$ ($1 \le idx_i \le n - 2$), where $idx_i$ is the index of left border of the segment for the $i$-th operation. You should print indices <span class="tex-font-style-bf">in order of performing operations</span>.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 100$) �� the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($3 \le n \le 500$) �� the length of $a$. The second line of the test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 500$), where $a_i$ is the $i$-th element $a$.</p><p>It is guaranteed that the sum of $n$ does not exceed $500$.</p>

## Output

<p>For each test case, print the answer: <span class="tex-font-style-tt">-1</span> on the only line if it is impossible to sort the given array using operations described in the problem statement, or the number of operations $ans$ on the first line and $ans$ integers $idx_1, idx_2, \dots, idx_{ans}$ ($1 \le idx_i \le n - 2$), where $idx_i$ is the index of left border of the segment for the $i$-th operation. You should print indices <span class="tex-font-style-bf">in order of performing operations</span>.</p>

## Samples

```input1
5
5
1 2 3 4 5
5
5 4 3 2 1
8
8 4 5 2 3 6 7 3
7
5 2 1 6 4 7 3
6
1 2 3 3 6 4
```

```output1
0

6
3 1 3 2 2 3 
13
2 1 1 6 4 2 4 3 3 4 4 6 6 
-1
4
3 3 4 4
```



