## Description

<div><p> </p><p>Gellyfish and Flower are playing a game.</p><p>The game consists of two arrays of $n$ integers $a_1,a_2,\ldots,a_n$ and $b_1,b_2,\ldots,b_n$, along with a binary string $c_1c_2\ldots c_n$ of length $n$.</p><p>There is also an integer $x$ which is initialized to $0$.</p><p>The game consists of $n$ rounds. For $i = 1,2,\ldots,n$, the round proceeds as follows:</p><ol> <li> If $c_i = \mathtt{0}$, Gellyfish will be the active player. Otherwise, if $c_i = \mathtt{1}$, Flower will be the active player. </li><li> The active player will perform <span class="tex-font-style-bf">exactly one</span> of the following operations: <ul> <li> Set $x:=x \oplus a_i$. </li><li> Set $x:=x \oplus b_i$. </li></ul> </li></ol><p>Here, $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>. </p><p>Gellyfish wants to minimize the final value of $ x $ after $ n $ rounds, while Flower wants to maximize it. </p><p>Find the final value of $ x $ after all $ n $ rounds if both players play optimally.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 10^5$)&nbsp;！ the number of rounds of the game.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i &lt; 2^{60}$).</p><p>The third line of each test case contains $n$ integers $b_1, b_2, \ldots, b_n$ ($0 \leq b_i &lt; 2^{60}$).</p><p>The fourth line of each test case contains a binary string $c$ of length $n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the final value of $ x $ after all $ n $ rounds.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 10^5$)&nbsp;！ the number of rounds of the game.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i &lt; 2^{60}$).</p><p>The third line of each test case contains $n$ integers $b_1, b_2, \ldots, b_n$ ($0 \leq b_i &lt; 2^{60}$).</p><p>The fourth line of each test case contains a binary string $c$ of length $n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the final value of $ x $ after all $ n $ rounds.</p>





```input1|2,3,4,5,10,11,12,13,18,19,20,21
5
1
0
2
0
2
12 2
13 3
11
3
6 1 2
6 2 3
010
4
1 12 7 2
4 14 4 2
0111
9
0 5 10 6 6 2 6 2 11
7 3 15 3 6 7 6 7 8
110010010
```




```output1
0
15
6
11
5
```



## Note

<p>In the first test case, there's only one round and Gellyfish is the active player of that round. Therefore, she will choose $a_1$, and the final value of $x$ is $0$.</p><p>In the second test case, Flower will be the active player in both rounds. She will choose $a_1$ and $b_2$, and the final value of $x$ is $a_1 \oplus b_2 = 15$. Flower may also choose $b_1$ and $a_2$ instead for the same result of $x=a_2 \oplus b_1 = 15$.</p><p>In the third test case, $a_1 = b_1$ so it doesn't matter what decision Gellyfish makes in the first round. In the second round:</p><ul> <li> If Flower chooses $a_2$, then $x$ will become $7$. Gellyfish will choose $b_3$ in the third round, so the final value of $x$ will be $4$. </li><li> Otherwise, Flower chooses $b_2$, then $x$ will become $4$. Gellyfish will choose $a_3$ in the third round, so the final value of $x$ will be $6$. </li></ul><p>Flower wants to maximize the final value of $x$, so Flower will choose $b_2$ in the second round. Therefore, the final value of $x$ will be $6$.</p>
