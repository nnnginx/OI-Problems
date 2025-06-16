<p>We consider a sequence <b>S<sub>1</sub></b> is <b>equal</b> to a sequence <b>S<sub>2</sub></b>, if and only if they satisfy the following conditions:</p>

<ul>
<li>The length of them are equal.
</li><li>Let <b>Len</b> be the length of them. For each i,j(1 &lt;= i, j &lt;= <b>Len</b>, i != j):If <b>S<sub>1</sub></b>[i] is smaller than <b>S<sub>1</sub></b>[j], <b>S<sub>2</sub></b>[i] must be smaller than <b>S<sub>2</sub></b>[j]; If <b>S<sub>1</sub></b>[i] is greater than <b>S<sub>1</sub></b>[j], <b>S<sub>2</sub></b>[i] must greater than <b>S<sub>2</sub></b>[j].
</li></ul>

<p>Now you are given a sequence <b>S</b> and another <b>N</b> sequences <b>T<sub>1</sub></b>, <b>T<sub>2</sub></b> бн. <b>T<sub>N</sub></b>.</p>
<p>We say position <b>i</b> is <b>OK</b>, if and only if <b>S</b>[1..<b>i</b>] contains a suffix which is <b>equal</b> to a sequence from { <b>T<sub>1</sub></b>, <b>T<sub>2</sub></b> ... <b>T<sub>N</sub></b> }. You need to print the positions which is <b>OK</b> in increasing order.</p>

<h3>Input</h3>

<p>Multiple test cases, the number of them(no more than 3) is given in the very first line.</p>
<p>For each test case:</p>
<ul>
<li>The first line contains an integer <b>M</b> (<b>M</b> &gt; 1) which denote the number of sequences. <b>i.e.</b> <b>M</b> = <b>N</b> + 1.
</li><li><b>M</b> * 2 lines follow, each two lines describe one sequence.For each two lines, the first line contains an integer <b>L</b> which denote the length of this sequence. The second line contains <b>L</b> integers(all the integers don't exceed 2<sup>31</sup>-1) that represent this sequence.
The first sequence described is <b>S</b>, the next <b>N</b> sequences represent <b>T<sub>1</sub></b> ... <b>T<sub>N</sub></b>.
</li><li>You can assume that there are no same integer in any one sequence.
</li><li>The length of <b>S</b> is no more than 400000, and the total length of <b>T</b> is no more than 100000.
</li></ul>

<h3>Output</h3>
<p>For each test case: Print the positions which is <b>OK</b> in increasing order.</p>


<h3>Example</h3>

<pre><b>Input:</b>
2
2
1
1
1
2
3
3
3 1 2
2
4 5
2
10 1

<b>Output:</b>
1
2
3
</pre>