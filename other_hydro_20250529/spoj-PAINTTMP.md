<p align="justify">The Painter's Studio is preparing mass production of paintings. Paintings are going to be made with aid of square matrices of various sizes. A matrix of size <i>i</i> consists of 2<i><sup>i</sup></i> rows and 2<i><sup>i</sup></i> columns. There are holes on intersections of some rows and columns. Matrix of size 0 has one hole. For <i>i</i> &gt; 0, matrix of size <i>i</i> is built of four squares of size 2<sup>(</sup><i><sup>i</sup></i><sup>-1)</sup>*2<sup>(</sup><i><sup>i</sup></i><sup>-1)</sup>. Look at the following figure:</p>
<p align="center"><img src="/content/ahven:malrys1.gif"></p>
<p align="justify">Both squares on the right side and the bottom-left square are matrices of size <i>i</i>-1. Top-left square has no holes. Pictures are constructed in the following way. First, we fix three non-negative integers <i>n</i>, <i>x</i>, <i>y</i>. Next, we take two matrices of size <i>n</i>, place one of them onto the other and shift the upper one <i>x</i> columns right and <i>y</i> rows up. We place such a pattern on a white canvas and cover the common part of matrices with the yellow paint. In this way we get yellow stains on the canvas in the places where the holes in both matrices agree.</p>

<h3>Example</h3>
<p align="justify">Consider two matrices of size 2.</p>
<p align="center"><img src="/content/ahven:malrys2.jpg"></p>
<p align="justify">The upper matrix was shifted 2 columns right and 2 rows up. There are three places where holes agree.</p>

<h3>Task</h3>
<p align="justify">Write a program that for each test case:</p>
<div align="justify">
<ul align="justify">
        <li align="justify">reads the sizes of two matrices and the numbers of columns and rows that the upper matrix should be shifted by, from the standard input;</li>
        <li align="justify">computes the number of yellow stains on the canvas;</li>
        <li align="justify">writes the result to the standard output.</li>
</ul>
</div>
<h3>Input</h3>
<p align="justify">The number of test cases <i>t</i> is in the first line of input, then <i>t</i> test cases follow separated by an empty line</p>
<p align="justify">There is one integer <i>n</i>, 0 &lt;= <i>n</i> &lt;= 100 in the first line of each test case. This number is the size of matrices used for production of paintings. In the second line there is one integer <i>x</i> and in the third line one integer <i>y</i>, where 0 &lt;= <i>x</i>,<i>y</i> &lt;= 2<i><sup>n</sup></i>. The integer <i>x</i> is the number of columns and <i>y</i> is the number of rows that the upper matrix should be shifted by.</p>

<h3>Output</h3>
<p align="justify">For each test case your program should produce one line with exactly one integer - the number of stains on the canvas.</p>

<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
2
2
2

<b><tt>Sample output:</tt></b>
3
</pre>