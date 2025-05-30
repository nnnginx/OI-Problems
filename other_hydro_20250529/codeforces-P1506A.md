## Description

<div><p>Polycarp found a rectangular table consisting of $n$ rows and $m$ columns. He noticed that each cell of the table has its number, obtained by the following algorithm <span class="tex-font-style-bf">"by columns"</span>: </p><ul> <li> cells are numbered starting from one; </li><li> cells are numbered from left to right by columns, and inside each column from top to bottom; </li><li> number of each cell is an integer one greater than in the previous cell. </li></ul><p>For example, if $n = 3$ and $m = 5$, the table will be numbered as follows:</p><p>$$ \begin{matrix} 1 &amp; 4 &amp; 7 &amp; 10 &amp; 13 \\ 2 &amp; 5 &amp; 8 &amp; 11 &amp; 14 \\ 3 &amp; 6 &amp; 9 &amp; 12 &amp; 15 \\ \end{matrix} $$</p><p>However, Polycarp considers such numbering inconvenient. He likes the numbering <span class="tex-font-style-bf">"by rows"</span>: </p><ul> <li> cells are numbered starting from one; </li><li> cells are numbered from top to bottom by rows, and inside each row from left to right; </li><li> number of each cell is an integer one greater than the number of the previous cell. </li></ul><p>For example, if $n = 3$ and $m = 5$, then Polycarp likes the following table numbering: $$ \begin{matrix} 1 &amp; 2 &amp; 3 &amp; 4 &amp; 5 \\ 6 &amp; 7 &amp; 8 &amp; 9 &amp; 10 \\ 11 &amp; 12 &amp; 13 &amp; 14 &amp; 15 \\ \end{matrix} $$</p><p>Polycarp doesn't have much time, so he asks you to find out what would be the cell number in the numbering <span class="tex-font-style-bf">"by rows"</span>, if in the numbering <span class="tex-font-style-bf">"by columns"</span> the cell has the number $x$?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$). Then $t$ test cases follow.</p><p>Each test case consists of a single line containing three integers $n$, $m$, $x$ ($1 \le n, m \le 10^6$, $1 \le x \le n \cdot m$), where $n$ and $m$ are the number of rows and columns in the table, and $x$ is the cell number.</p><p>Note that the numbers in some test cases do not fit into the $32$-bit integer type, so you must use at least the $64$-bit integer type of your programming language.</p></div><div class="output-specification"><p>For each test case, output the cell number in the numbering <span class="tex-font-style-bf">"by rows"</span>.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$). Then $t$ test cases follow.</p><p>Each test case consists of a single line containing three integers $n$, $m$, $x$ ($1 \le n, m \le 10^6$, $1 \le x \le n \cdot m$), where $n$ and $m$ are the number of rows and columns in the table, and $x$ is the cell number.</p><p>Note that the numbers in some test cases do not fit into the $32$-bit integer type, so you must use at least the $64$-bit integer type of your programming language.</p>

## Output

<p>For each test case, output the cell number in the numbering <span class="tex-font-style-bf">"by rows"</span>.</p>

## Samples

```input1
5
1 1 1
2 2 3
3 5 11
100 100 7312
1000000 1000000 1000000000000
```

```output1
1
2
9
1174
1000000000000
```



