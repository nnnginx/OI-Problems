## Description

<div><p>Vanya has a table consisting of <span class="tex-span">100</span> rows, each row contains <span class="tex-span">100</span> cells. The rows are numbered by integers from <span class="tex-span">1</span> to <span class="tex-span">100</span> from bottom to top, the columns are numbered from <span class="tex-span">1</span> to <span class="tex-span">100</span> from left to right. </p><p>In this table, Vanya chose <span class="tex-span"><i>n</i></span> rectangles with sides that go along borders of squares (some rectangles probably occur multiple times). After that for each cell of the table he counted the number of rectangles it belongs to and wrote this number into it. Now he wants to find the sum of values in all cells of the table and as the table is too large, he asks you to help him find the result.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of rectangles.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains four integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub> ≤ 100</span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i><sub class="lower-index">2</sub> ≤ 100)</span>, where <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> are the number of the column and row of the lower left cell and <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> are the number of the column and row of the upper right cell of a rectangle.</p></div><div class="output-specification"><p>In a single line print the sum of all values in the cells of the table.</p></div>


## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of rectangles.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains four integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub> ≤ 100</span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i><sub class="lower-index">2</sub> ≤ 100)</span>, where <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> are the number of the column and row of the lower left cell and <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> are the number of the column and row of the upper right cell of a rectangle.</p>


## Output

<p>In a single line print the sum of all values in the cells of the table.</p>


## Samples

```input1
2
1 1 2 3
2 2 3 3

```

```output1
10

```






```input2
2
1 1 3 3
1 1 3 3

```

```output2
18

```




## Note

<p>Note to the first sample test:</p><p>Values of the table in the first three rows and columns will be as follows:</p><p><span class="tex-span">121</span></p><p><span class="tex-span">121</span></p><p><span class="tex-span">110</span></p><p>So, the sum of values will be equal to <span class="tex-span">10</span>.</p><p>Note to the second sample test:</p><p>Values of the table in the first three rows and columns will be as follows:</p><p><span class="tex-span">222</span></p><p><span class="tex-span">222</span></p><p><span class="tex-span">222</span></p><p>So, the sum of values will be equal to <span class="tex-span">18</span>.</p>

