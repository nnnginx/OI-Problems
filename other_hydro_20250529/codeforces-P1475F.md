## Description

<div><p>You are given two binary square matrices $a$ and $b$ of size $n \times n$. A matrix is called binary if each of its elements is equal to $0$ or $1$. You can do the following operations on the matrix $a$ <span class="tex-font-style-bf">arbitrary</span> number of times (0 or more): </p><ul> <li> vertical <span class="tex-font-style-tt">xor</span>. You choose the number $j$ ($1 \le j \le n$) and for all $i$ ($1 \le i \le n$) do the following: $a_{i, j} := a_{i, j} \oplus 1$ ($\oplus$&nbsp;！ is the operation <a href="https://en.wikipedia.org/wiki/Exclusive_or"><span class="tex-font-style-tt">xor</span></a> (exclusive or)). </li><li> horizontal <span class="tex-font-style-tt">xor</span>. You choose the number $i$ ($1 \le i \le n$) and for all $j$ ($1 \le j \le n$) do the following: $a_{i, j} := a_{i, j} \oplus 1$. </li></ul><p>Note that the elements of the $a$ matrix change after each operation.</p><p>For example, if $n=3$ and the matrix $a$ is: $$ \begin{pmatrix} 1 &amp; 1 &amp; 0 \\ 0 &amp; 0 &amp; 1 \\ 1 &amp; 1 &amp; 0 \end{pmatrix} $$ Then the following sequence of operations shows an example of transformations: </p><ul> <li> vertical <span class="tex-font-style-tt">xor</span>, $j=1$. $$ a= \begin{pmatrix} 0 &amp; 1 &amp; 0 \\ 1 &amp; 0 &amp; 1 \\ 0 &amp; 1 &amp; 0 \end{pmatrix} $$ </li><li> horizontal <span class="tex-font-style-tt">xor</span>, $i=2$. $$ a= \begin{pmatrix} 0 &amp; 1 &amp; 0 \\ 0 &amp; 1 &amp; 0 \\ 0 &amp; 1 &amp; 0 \end{pmatrix} $$ </li><li> vertical <span class="tex-font-style-tt">xor</span>, $j=2$. $$ a= \begin{pmatrix} 0 &amp; 0 &amp; 0 \\ 0 &amp; 0 &amp; 0 \\ 0 &amp; 0 &amp; 0 \end{pmatrix} $$ </li></ul><p>Check if there is a sequence of operations such that the matrix $a$ becomes equal to the matrix $b$.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \leq t \leq 1000$)&nbsp;！ the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case contains one integer $n$ ($1 \leq n \leq 1000$)&nbsp;！ the size of the matrices.</p><p>The following $n$ lines contain strings of length $n$, consisting of the characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>'&nbsp;！ the description of the matrix $a$.</p><p>An empty line follows.</p><p>The following $n$ lines contain strings of length $n$, consisting of the characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>'&nbsp;！ the description of the matrix $b$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $1000$.</p></div><div class="output-specification"><p>For each test case, output on a separate line: </p><ul> <li> "<span class="tex-font-style-tt">YES</span>", there is such a sequence of operations that the matrix $a$ becomes equal to the matrix $b$; </li><li> "<span class="tex-font-style-tt">NO</span>" otherwise. </li></ul><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will be recognized as positive).</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \leq t \leq 1000$)&nbsp;！ the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case contains one integer $n$ ($1 \leq n \leq 1000$)&nbsp;！ the size of the matrices.</p><p>The following $n$ lines contain strings of length $n$, consisting of the characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>'&nbsp;！ the description of the matrix $a$.</p><p>An empty line follows.</p><p>The following $n$ lines contain strings of length $n$, consisting of the characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>'&nbsp;！ the description of the matrix $b$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $1000$.</p>

## Output

<p>For each test case, output on a separate line: </p><ul> <li> "<span class="tex-font-style-tt">YES</span>", there is such a sequence of operations that the matrix $a$ becomes equal to the matrix $b$; </li><li> "<span class="tex-font-style-tt">NO</span>" otherwise. </li></ul><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will be recognized as positive).</p>

## Samples

```input1
3
3
110
001
110

000
000
000
3
101
010
101

010
101
010
2
01
11

10
10
```

```output1
YES
YES
NO
```




## Note

<p>The first test case is explained in the statements.</p><p>In the second test case, the following sequence of operations is suitable: </p><ul> <li> horizontal <span class="tex-font-style-tt">xor</span>, $i=1$; </li><li> horizontal <span class="tex-font-style-tt">xor</span>, $i=2$; </li><li> horizontal <span class="tex-font-style-tt">xor</span>, $i=3$; </li></ul><p>It can be proved that there is no sequence of operations in the third test case so that the matrix $a$ becomes equal to the matrix $b$.</p>
