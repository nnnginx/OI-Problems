<p>A student is always bored during his math classes. As the teacher won't let him sleep, he finds something else to do: try to find patterns in the numbers written on the board! Currently, he's spending his time trying to find Hi&amp;Lo subsequences.</p>
<p>Intuitively, a Hi&amp;Lo sequence is any sequence that has consecutive differences with opposite signs, that is, if the first number is greater than the second, then the second is smaller than the third, the third is greater than the fourth, and so on.</p>
<p>Formally, let x[1], x[2], ..., x[n] be the numbers written on the board. A Hi&amp;Lo subsequence of length k that only uses elements from A to B is a sequence of indices a<sub>1</sub>, a<sub>2</sub>, ..., a<sub>k</sub>&nbsp;such that:</p>
<ol>
<li>B&nbsp;<span style="font-family: verdana, arial, helvetica, code2000, sans-serif; font-size: small;">��</span>&nbsp;a<sub>k</sub>&nbsp;&gt; ... &gt;&nbsp;a<sub>2</sub>&nbsp;&gt;&nbsp;a<sub>1 <span style="font-family: verdana, arial, helvetica, code2000, sans-serif; font-size: small;">��</span>&nbsp;</sub>A</li>
<li>x[a<sub>i</sub>]- x[a<sub>i-1</sub>] != 0, for 1 &lt; i &lt;= k</li>
<li>( x[a<sub>i</sub>]<sub>&nbsp;</sub>- x[a<sub>i-1</sub>] )( x[a<sub>i+1</sub>] - x[a<sub>i</sub>] ) &lt; 0, for 1 &lt; i &lt; k&nbsp;</li>
</ol>
<p>Note that every sequence with only one element is a Hi&amp;Lo sequence.</p>
<p>However, as the amount of numbers increases, finding a big subsequence is getting harder and harder, so he asked you to create a program to help him and quickly find the largest Hi&amp;Lo subsequence in a given interval.&nbsp;</p>
<h3>Input</h3>
<p>The input contains several test cases. A test case begins with a line containing integers <strong>N </strong>(1&nbsp;<span style="font-family: verdana, arial, helvetica, code2000, sans-serif; font-size: small; background-color: #efefef;">��&nbsp;</span>N&nbsp;<span style="font-family: verdana, arial, helvetica, code2000, sans-serif; font-size: small; background-color: #efefef;">��&nbsp;</span>100000) &nbsp;and&nbsp;<strong>M </strong>(1&nbsp;<span style="font-family: verdana, arial, helvetica, code2000, sans-serif; font-size: small; background-color: #efefef;">��</span>&nbsp;M&nbsp;<span style="font-family: verdana, arial, helvetica, code2000, sans-serif; font-size: small; background-color: #efefef;">��</span>&nbsp;10000), separated by spaces. On the second line there are <strong>N</strong>&nbsp;positive integers, the initial state of the board.&nbsp;<strong>M</strong>&nbsp;lines follow, each with an instruction. Instructions can be of two kinds:</p>
<p>1) q A B: Print the length of the longest high &amp; low subsequence only using elements in positions from A to B, inclusive. You may assume that 1 <span style="font-family: verdana, arial, helvetica, code2000, sans-serif; font-size: small; background-color: #efefef;">��&nbsp;</span>A <span style="font-family: verdana, arial, helvetica, code2000, sans-serif; font-size: small; background-color: #efefef;">��</span>&nbsp;B <span style="font-family: verdana, arial, helvetica, code2000, sans-serif; font-size: small; background-color: #efefef;">��</span>&nbsp;N.&nbsp;</p>
<p>2) m A B: Modify the Ath element of the sequence to the positive integer B. You may assume that 1 <span style="font-family: verdana, arial, helvetica, code2000, sans-serif; font-size: small; background-color: #efefef;">��</span>&nbsp;A <span style="font-family: verdana, arial, helvetica, code2000, sans-serif; font-size: small; background-color: #efefef;">��</span>&nbsp;N.&nbsp;</p>
<p>No number on the board will ever exceed 10<sup>9</sup>.&nbsp;There is a blank line after each test case. The last test case is followed by a line containing two zeros.</p>
<h3>Output</h3>
<p>For each instruction of type 1, print a line containing an integer, the answer to the query. After each test, print a blank line.&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 470px; width: 1px; height: 1px; overflow: hidden;">5 7</div>5 7
1 2 3 4 5
q 2 4
m 3 1
q 2 4
m 3 2
q 2 4
m 4 2
q 2 4</pre>
<pre>0 0</pre>
<pre><strong>Output:</strong>
2
3
2
1</pre>