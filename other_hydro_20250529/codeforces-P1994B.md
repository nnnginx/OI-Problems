## Description

<div><p>Vova really loves the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">XOR</a> operation (denoted as $\oplus$). Recently, when he was going to sleep, he came up with a fun game.</p><p>At the beginning of the game, Vova chooses two binary sequences $s$ and $t$ of length $n$ and gives them to Vanya. A binary sequence is a sequence consisting only of the numbers $0$ and $1$. Vanya can choose integers $l, r$ such that $1 \leq l \leq r \leq n$, and for all $l \leq i \leq r$ <span class="tex-font-style-bf">simultaneously</span> replace $s_i$ with $s_i \oplus s_{i - l + 1}$, where $s_i$ is the $i$-th element of the sequence $s$.</p><p>In order for the game to be <span class="tex-font-style-it">interesting</span>, there must be a possibility to win. Vanya wins if, with an <span class="tex-font-style-bf">unlimited</span> number of actions, he can obtain the sequence $t$ from the sequence $s$. Determine if the game will be <span class="tex-font-style-it">interesting</span> for the sequences $s$ and $t$.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains an integer $q$ ($1 \le q \le 10^{4}$)&nbsp;！ the number of test cases. Then follows the description of the test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;！ the length of the sequences $s$ and $t$.</p><p>The second line of each test case contains a binary sequence $s$ of length $n$.</p><p>The third line of each test case contains a binary sequence $t$ of length $n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">Yes</span>" if the game will be <span class="tex-font-style-it">interesting</span>, otherwise output "<span class="tex-font-style-tt">No</span>".</p><p>You can output each letter in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains an integer $q$ ($1 \le q \le 10^{4}$)&nbsp;！ the number of test cases. Then follows the description of the test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;！ the length of the sequences $s$ and $t$.</p><p>The second line of each test case contains a binary sequence $s$ of length $n$.</p><p>The third line of each test case contains a binary sequence $t$ of length $n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">Yes</span>" if the game will be <span class="tex-font-style-it">interesting</span>, otherwise output "<span class="tex-font-style-tt">No</span>".</p><p>You can output each letter in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p>





```input1|2,3,4,8,9,10,14,15,16
6
1
0
1
7
0110100
0110100
9
100101010
101111110
4
0011
1011
4
0100
0001
8
10110111
01100000
```




```output1
NO
YES
YES
NO
YES
YES
```



## Note

<p>In the first test case, Vanya will not be able to change the sequence $s$ with the only possible action of choosing $l = r = 1$.</p><p>In the second test case, the sequences $s$ and $t$ are already equal.</p><p>In the third test case, Vanya can act as follows:</p><ol><li> Choose $l = 3$ and $r = 5$, then $s$ will become $\mathtt{101101010}$.</li><li> Choose $l = 5$ and $r = 6$, then $s$ will become $\mathtt{101111010}$.</li><li> Choose $l = 7$ and $r = 7$, then $s$ will become $\mathtt{101111110}$.</li></ol>
