<p>Alan loves to construct a stack of building bricks. His stack consists of many cuboids with square
base. All cuboids have the same height 1. Alan puts the consecutive cuboids one over another.
</p><p>Recently in math class, the concept of volume was introduced to Alan. Consequently, he wants to
compute the volume of his stack now. The lengths of cuboids bases (from top to bottom) are constructed
by Alan in the following way:</p>
<div align="justify">
    <ul>
        <li>
	 Length of edge of the first square is one. i.e. <b>a<sub>1</sub></b> = 1.
        </li><li>
        Next, Alan fixes the length of the edge of the second square <b>a<sub>2</sub></b>.
        </li><li>
        Next, Alan calculates the length <b>a<sub>n</sub></b> (n &gt; 2) by <b>2*a<sub>2</sub>*a<sub>n-1</sub> - a<sub>n-2</sub></b>. Do not ask why he chose such a formula; let us just say that he is a really peculiar young fellow.
        </li>
    </ul>
</div>
<p>For example, if Alan fixes <b>a<sub>2</sub></b> = 2, then <b>a<sub>3</sub></b> = 7. If Alan fixes <b>a<sub>2</sub></b> = 1, then <b>a<sub>n</sub></b> = 1 holds for all n.
</p><p>Now Alan wonders if he can calculate the volume of stack of <b>N</b> consecutive building bricks. Help
Alan and write the program that computes this volume. Since it can be quite large, it is enough to
compute the answer modulo given natural number <b>m</b>.</p>
<h3>Input</h3>
<p>The input contains several test cases. The first line contains the number t (t &lt;= 100000) denoting the number
of test cases. Then t test cases follow. Each of them is given in a separate line containing three integers
<b>a<sub>2</sub></b>, <b>N</b>, <b>m</b> (1 &lt;= <b>a<sub>2</sub></b>, <b>m</b> &lt;= 10<sup>9</sup>, 2 &lt;= <b>N</b> &lt;= 10<sup>9</sup>) separated by a single space.</p>
<h3>Output</h3>
<p>For each test case compute the volume of stack of <b>N</b> consecutive bricks constructed by Alan
according to steps 1 to 3 and output its remainder modulo <b>m</b>.</p>
<h3>Example</h3>
<pre><b>Input:</b>
3
2 3 100
1 4 1000
3 3 1000000000

<b>Output:</b>
54
4
299
</pre>
<p><b>Warning: large input/output data, be careful with certain languages</b>
</p><p><b>Warning: A naive algorithm won't terminate in even 2 minutes.</b></p>