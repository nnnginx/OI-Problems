<p>Given a sequence of <i>N</i> ordered pairs of positive integers (<i>A<sub>i</sub></i>, <i>B<sub>i</sub></i>), you have to 

partition it into several contiguous parts. Let <i>p</i> be the number of these parts, whose boundaries are 

(<i>l</i><sub>1</sub>, <i>r</i><sub>1</sub>), (<i>l</i><sub>2</sub>, <i>r</i><sub>2</sub>), ... ,(<i>l<sub>p</sub></i>, 

<i>r<sub>p</sub></i>), which satisfy <i>l<sub>i </sub></i>=<i> r<sub>i-</sub></i><sub>1 </sub>+ 1, <i>l<sub>i 

</sub></i>&lt;=<i> r<sub>i</sub></i>, <i>l</i><sub>1<i> </i></sub>= 1, <i>r<sub>p </sub></i>= <i>n</i>. The parts themselves 

also satisfy the following restrictions:</p><ol><li><p>For any two pairs (<i>A<sub>p</sub></i>, <i>B<sub>p</sub></i>), 

(<i>A<sub>q</sub></i>,<i> B<sub>q</sub></i>), where (<i>A<sub>p</sub></i>,<i> B<sub>p</sub></i>) is belongs to the 

<i>T<sub>p</sub></i>th part and (<i>A<sub>q</sub></i>, <i>B<sub>q</sub></i>) the <i>T<sub>q</sub></i>th part. If 

<i>T<sub>p</sub> </i>&lt;<i> T<sub>q</sub></i>, then <i>B<sub>p </sub></i>&gt;<i> A<sub>q</sub></i>.</p></li><li><p>Let 

<i>M<sub>i</sub></i> be the maximum <i>A</i>-component of elements in the <i>i</i>th part, say</p><p><i>M<sub>i</sub></i> = max

{<i>A<sub>l<sub>i</sub></sub></i>, 

<i>A<sub>l<sub>i+</sub></sub></i><sub><sub>1</sub></sub>, ..., <i>A<sub>r<sub>i</sub></sub></i>}, 1 &lt;= <i>i</i> &lt;= 

<i>p</i></p><p>it is provided that</p><p><img src="../../content/crazyb0y:SEQPAR2_1.bmp"><br> 

where Limit is a given integer.</p></li></ol><p>Let <i>S<sub>i</sub></i> be the sum of <i>B</i>-components of elements 

in the <i>i</i>th part. </p><p>Now I want to minimize the value</p><p>max{<i>S<sub>i</sub></i>:1 &lt;= <i>i</i> &lt;= 

p} </p><p>Could you tell me the minimum?

</p><h3>Input</h3>
<p>The input contains exactly one test case. The first line of input contains two positive integers N (N &lt;= 50000), Limit 

(Limit &lt;= 2<sup>31</sup>-1). Then follow N lines each contains a positive integers pair (<i>A</i>, <i>B</i>). It's always 

guaranteed that</p><p> max{<i>A</i><sub>1</sub>, <i>A</i><sub>2</sub>, ..., <i>A<sub>n</sub></i>} &lt;= Limit<br><img src="../../content/crazyb0y:SEQPAR2_2.bmp">

</p><h3>Output</h3>
<p>Output the minimum target value.

</p><h3>Example</h3>

<pre><b>Input:</b>
4 6
4 3
3 5
2 5
2 4

<b>Output:</b>
9

</pre>
<h3>Explanation</h3>
<p>An available assignment is the first two pairs are assigned into the first part and the last two pairs are assigned into 

the second part. Then <i>B</i><sub>1</sub> &gt; <i>A</i><sub>3</sub>, <i>B</i><sub>1</sub> &gt; <i>A</i><sub>4</sub>, 

<i>B</i><sub>2</sub> &gt; <i>A</i><sub>3</sub>, <i>B</i><sub>2</sub> &gt; <i>A</i><sub>4</sub>, max{<i>A</i><sub>1</sub>, 

<i>A</i><sub>2</sub>}+max{<i>A</i><sub>3</sub>, <i>A</i><sub>4</sub>} &lt;= 6, and minimum max

{<i>B</i><sub>1</sub>+<i>B</i><sub>2</sub>, <i>B</i><sub>3</sub>+<i>B</i><sub>4</sub>}=9.
</p>