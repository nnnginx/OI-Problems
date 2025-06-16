## Description

<div><p>Akito still has nowhere to live, and the price for a small room is everywhere. For this reason, Akito decided to get a job at a bank as a key creator for storages.</p><p>In this magical world, everything is different. For example, the key for a storage with the code $(n, x)$ is an array $a$ of length $n$ such that:</p><ul> <li> $a_1 \ | \ a_2 \ | \ a_3 \ | \ \ldots \ | \ a_n = x$, where $a \ | \ b$ is the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#OR">bitwise "OR"</a> of numbers $a$ and $b$.</li><li> $\text{MEX}(\{ a_1, a_2, a_3, \ldots, a_n \})$$^{\text{∗}}$ is maximized among all such arrays. </li></ul><p>Akito diligently performed his job for several hours, but suddenly he got a headache. Substitute for him for an hour; for the given $n$ and $x$, create any key for the storage with the code $(n, x)$.</p><div class="statement-footnote"><p>$^{\text{∗}}$$\text{MEX}(S)$ is the minimum non-negative integer $z$ such that $z$ is not contained in the set $S$ and all $0 \le y &lt; z$ are contained in $S$.</p></div></div><div class="input-specification"><p>The first line contains the number $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>In the only line of each test case, two numbers $n$ and $x$ ($1 \le n \le 2 \cdot 10^5, 0 \le x &lt; 2^{30}$) are given — the length of the array and the desired value of the bitwise "OR".</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output $n$ integers $a_i$ ($0 \le a_i &lt; 2^{30}$) — the elements of the key array that satisfy all the conditions.</p><p>If there are multiple suitable arrays, output any of them.</p></div>

## Input

<p>The first line contains the number $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>In the only line of each test case, two numbers $n$ and $x$ ($1 \le n \le 2 \cdot 10^5, 0 \le x &lt; 2^{30}$) are given — the length of the array and the desired value of the bitwise "OR".</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output $n$ integers $a_i$ ($0 \le a_i &lt; 2^{30}$) — the elements of the key array that satisfy all the conditions.</p><p>If there are multiple suitable arrays, output any of them.</p>





```input1|2,4,6,8,10
9
1 69
7 7
5 7
7 3
8 7
3 52
9 11
6 15
2 3
```




```output1
69
6 0 3 4 1 2 5
4 1 3 0 2
0 1 2 3 2 1 0
7 0 6 1 5 2 4 3
0 52 0
0 1 8 3 0 9 11 2 10
4 0 3 8 1 2
0 3
```


