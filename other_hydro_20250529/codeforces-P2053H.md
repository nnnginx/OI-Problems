## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">I shall be looking for you who would be out of Existence.</span></div><div class="epigraph-source">！ HyuN, <a href="https://soundcloud.com/k-sounds-studio/g2r2018-hyun-disorder-feat-yuri"><span class="tex-font-style-it">Disorder</span></a></div></div><p><span class="tex-font-style-it">There are always many repetitive tasks in life. Iris always dislikes them, so she refuses to repeat them. However, time cannot be turned back; we only have to move forward.</span></p><p>Formally, Iris has an integer sequence $a_1, a_2, \ldots, a_n$, where each number in the sequence is between $1$ and $w$, inclusive. It is guaranteed that $w \geq 2$.</p><p>Iris defines an <span class="tex-font-style-it">operation</span> as selecting two numbers $a_i, a_{i+1}$ satisfying $a_i = a_{i+1}$, and then changing them to two arbitrary integers within the range $[1, w]$. Iris does not like equality, so she must guarantee that $a_i \neq a_{i+1}$ after the operation. Two identical pairs $a_i, a_{i+1}$ can be selected multiple times.</p><p>Iris wants to know the maximum possible sum of all elements of $a$ after several (possible, zero) <span class="tex-font-style-it">operations</span>, as well as the minimum number of <span class="tex-font-style-it">operations</span> required to achieve this maximum value.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 10^5$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $w$ ($1 \leq n \leq 2\cdot 10^5$, $2 \leq w \leq 10^8$)&nbsp;！ the length of the array, and the maximum allowed value of the elements.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq w$)&nbsp;！ the elements in the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, output two integers&nbsp;！ the maximum possible sum of all elements of $a$ and the minimum number of operations required, respectively.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 10^5$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $w$ ($1 \leq n \leq 2\cdot 10^5$, $2 \leq w \leq 10^8$)&nbsp;！ the length of the array, and the maximum allowed value of the elements.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq w$)&nbsp;！ the elements in the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$.</p>

## Output

<p>For each test case, output two integers&nbsp;！ the maximum possible sum of all elements of $a$ and the minimum number of operations required, respectively.</p>





```input1|2,3
2
5 8
1 2 3 4 5
7 5
3 1 2 3 4 1 1
```




```output1
15 0
34 6
```



## Note

<p>In the first test case, no <span class="tex-font-style-it">operation</span> can be performed so the answers are $\sum a_i = 15$ and $0$, respectively.</p><p>In the second test case, the <span class="tex-font-style-it">operations</span> can be performed as follows:</p><p>$$[3, 1, 2, 3, 4, \underline{1, 1}] \rightarrow [3, 1, 2, 3, \underline{4, 4}, 5] \rightarrow [3, 1, 2, \underline{3, 3}, 5, 5] \rightarrow [3, 1, \underline{2, 2}, 5, 5, 5] \rightarrow [3, \underline{1, 1}, 5, 5, 5, 5] \rightarrow [\underline{3, 3}, 5, 5, 5, 5, 5] \rightarrow [4, 5, 5, 5, 5, 5, 5]$$</p><p>It can be shown this is optimal, so we should output $\sum a_i = 34$ and the number of <span class="tex-font-style-it">operations</span>, $6$, respectively.</p>
