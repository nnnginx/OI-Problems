<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/MBRACKET/en/">English</a></td>
<td width="50%"><a href="/problems/MBRACKET/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<pre>Lets observe sequences made only of round and square brackets, i.e. <br>characters '( ) [ ]'. <br>A sequence of brackets is regular if it satisfies this inductive definition: <br>1. '( )' and '[ ]' are regular sequences <br>2. If A is regular, then (A) and [A] are regular sequences <br>3. If A and B are regular, then AB is regular sequence.<br><br>For example '( ) ( ) [ ]', '( [ ] ) [ ( ) ]' and '[ ( ( ) ) ] [ ]' are regular, <br>while '(', '] [', '[ ( ]' and '( [ ) ]' are not regular. <br>The sequence of brackets is given. <br><br>In every step, one bracket is inserted  at the beginning  or at the end of the <br>sequence (round or square, left or right). <br><br>Write a program that will,  after each step, determine  the length of the  <br>shortest regular subsequence of consecutive characters that contains the <br>bracket added in that step. <br> <br></pre>
<h3>Input</h3>
<pre>First line contains initial sequence of brackets, whose length is at most <br>100,000 characters. <br><br>Next line contains integer N, 1 ¡Ü N ¡Ü 100,000, a number of steps. <br><br>In each of next N lines there are integer A and character C, separated by a <br>single space. If A is zero (0), than character C is inserted at the <br>beginning, and if A is one (1) then C is inserted at the end. <br></pre>
<h3>Output</h3>
<pre>In each of N lines, you should write the length of subsequence after<br>that step. If there is no such subsequence, write number 0. <br></pre>
<h3>Sample</h3>
<pre>input <br>[]) <br>3 <br>0 ) <br>0 ( <br>0 ( <br>output <br>0 <br>2 <br>6 <br><br>input <br>(] <br>3 <br>1 ) <br>0 ) <br>0 ( <br>output <br>0 <br>0 <br>2 <br></pre>
<p> </p>