## Description

<div><p>In the upcoming year, there will be many team olympiads, so the teachers of "T-generation" need to assemble a team of three pupils to participate in them. Any three pupils will show a worthy result in any team olympiad. But winning the olympiad is only half the battle; first, you need to get there...</p><p>Each pupil has an independence level, expressed as an integer. In "T-generation", there is exactly one student with each independence levels from $l$ to $r$, inclusive. For a team of three pupils with independence levels $a$, $b$, and $c$, the value of their team independence is equal to $(a \oplus b) + (b \oplus c) + (a \oplus c)$, where $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>. </p><p>Your task is to choose any trio of students with the maximum possible team independence.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case set contains two integers $l$ and $r$ ($0 \le l, r &lt; 2^{30}$, $r - l &gt; 1$)&nbsp;！ the minimum and maximum independence levels of the students.</p></div><div class="output-specification"><p>For each test case set, output three pairwise distinct integers $a, b$, and $c$, such that $l \le a, b, c \le r$ and the value of the expression $(a \oplus b) + (b \oplus c) + (a \oplus c)$ is maximized. If there are multiple triples with the maximum value, any of them can be output.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case set contains two integers $l$ and $r$ ($0 \le l, r &lt; 2^{30}$, $r - l &gt; 1$)&nbsp;！ the minimum and maximum independence levels of the students.</p>

## Output

<p>For each test case set, output three pairwise distinct integers $a, b$, and $c$, such that $l \le a, b, c \le r$ and the value of the expression $(a \oplus b) + (b \oplus c) + (a \oplus c)$ is maximized. If there are multiple triples with the maximum value, any of them can be output.</p>





```input1|2,4,6,8
8
0 2
0 8
1 3
6 22
128 137
69 98
115 127
0 1073741823
```




```output1
1 2 0
8 7 1
2 1 3
7 16 11
134 132 137
98 85 76
123 121 118
965321865 375544086 12551794
```



## Note

<p>In the first test case, the only suitable triplet of numbers ($a, b, c$) (up to permutation) is ($0, 1, 2$).</p><p>In the second test case, one of the suitable triplets is ($8, 7, 1$), where $(8 \oplus 7) + (7 \oplus 1) + (8 \oplus 1) = 15 + 6 + 9 = 30$. It can be shown that $30$ is the maximum possible value of $(a \oplus b) + (b \oplus c) + (a \oplus c)$ for $0 \le a, b, c \le 8$.</p>
