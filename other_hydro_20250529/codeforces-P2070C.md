## Description

<div><p>You are given a strip, consisting of $n$ cells, all cells are initially colored red.</p><p>In one operation, you can choose a segment of consecutive cells and paint them <span class="tex-font-style-bf">blue</span>. Before painting, the chosen cells can be either red or blue. Note that it is not possible to paint them red. You are allowed to perform at most $k$ operations (possibly zero).</p><p>For each cell, the desired color after all operations is specified: red or blue.</p><p>It is clear that it is not always possible to satisfy all requirements within $k$ operations. Therefore, for each cell, a penalty is also specified, which is applied if the cell ends up the wrong color after all operations. For the $i$-th cell, the penalty is equal to $a_i$.</p><p>The penalty of the final painting is calculated as the <span class="tex-font-style-bf">maximum penalty</span> among all cells that are painted the wrong color. If there are no such cells, the painting penalty is equal to $0$.</p><p>What is the minimum penalty of the final painting that can be achieved?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 3 \cdot 10^5$; $0 \le k \le n$)&nbsp;！ the length of the strip and the maximum number of operations.</p><p>The second line contains a string $s$, consisting of $n$ characters '<span class="tex-font-style-tt">R</span>' and/or '<span class="tex-font-style-tt">B</span>'. '<span class="tex-font-style-tt">R</span>' means that the cell should be painted red. '<span class="tex-font-style-tt">B</span>' means that the cell should be painted blue.</p><p>The third line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;！ the penalty for each cell.</p><p>The sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;！ the minimum penalty of the final painting.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 3 \cdot 10^5$; $0 \le k \le n$)&nbsp;！ the length of the strip and the maximum number of operations.</p><p>The second line contains a string $s$, consisting of $n$ characters '<span class="tex-font-style-tt">R</span>' and/or '<span class="tex-font-style-tt">B</span>'. '<span class="tex-font-style-tt">R</span>' means that the cell should be painted red. '<span class="tex-font-style-tt">B</span>' means that the cell should be painted blue.</p><p>The third line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;！ the penalty for each cell.</p><p>The sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single integer&nbsp;！ the minimum penalty of the final painting.</p>





```input1|2,3,4,8,9,10,14,15,16
5
4 1
BRBR
9 3 5 4
4 1
BRBR
9 5 3 4
4 2
BRBR
9 3 5 4
10 2
BRBRBBRRBR
5 1 2 4 5 3 6 1 5 4
5 5
RRRRR
5 3 1 2 4
```




```output1
3
3
0
4
0
```



## Note

<p>In the first test case, you can paint the cells from $1$ to $3$. The painting will be <span class="tex-font-style-tt">BBBR</span>. So, only cell $2$ is painted the wrong color. Therefore, the penalty for it is the final penalty and equals $3$.</p><p>In the second test case, the painting <span class="tex-font-style-tt">BBBR</span> will now result in a penalty of $5$. However, if you paint the cells from $1$ to $1$, resulting in <span class="tex-font-style-tt">BRRR</span>, then only cell $3$ is painted the wrong color. The final penalty is $3$.</p><p>In the third test case, you can paint the cells from $1$ to $1$ and from $3$ to $3$. Then all cells will be the correct color, the penalty equals $0$.</p>
