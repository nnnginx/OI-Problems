<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/LIS2VN/en/">English</a></td> 
<td width="50%"><a href="/problems/LIS2VN/vn/">Vietnamese</a></td> 
</tr></tbody></table>


<p>Given a sequence of <b>N</b> pairs of integers, find the length of the <b>longest increasing subsequence</b> of it. 
</p><p>An <b>increasing sequence</b> <i>A<sub>1</sub>..A<sub>n</sub></i> is a sequence such that for every <i> i &lt; j</i>, <i>A<sub>i</sub> &lt; A<sub>j</sub></i>. 

</p><p>A <b>subsequence</b> of a sequence is a sequence that appears in the same relative order, but not necessarily contiguous. 
</p><p>A pair of integers <i> (x<sub>1</sub>, y<sub>1</sub>)</i> is less than <i> (x<sub>2</sub>, y<sub>2</sub>)</i> <b>if</b> <i>x<sub>1</sub> &lt; x<sub>2</sub></i> and <i> y<sub>1</sub> &lt; y<sub>2</sub></i>. 


</p><h3>Input</h3>
<p>The first line of input contains an integer <b> N</b> (2 ¡Ü <b> N</b> ¡Ü 100000).
</p><p>The following <b> N</b> lines consist of <b> N</b> pairs of integers <i>(x<sub>i</sub>, y<sub>i</sub>)</i> (-10<sup>9</sup> ¡Ü <i>x<sub>i</sub>, y<sub>i</sub></i> ¡Ü 10<sup>9</sup>).


</p><h3>Output</h3>
<p>The output contains an integer: the length of the longest increasing subsequence of the given sequence.  

</p><h3>Example</h3>

<pre><b>Input:</b>
8
1 3
3 2
1 1
4 5
6 3
9 9
8 7
7 6

<b>Output:</b>
3
</pre>

<p>Original problem: <a href="http://www.spoj.com/problems/LIS2/">http://www.spoj.com/problems/LIS2/</a>.</p>