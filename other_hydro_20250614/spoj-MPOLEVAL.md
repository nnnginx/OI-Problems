<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/MPOLEVAL/en/">English</a></td>
<td width="50%"><a href="/problems/MPOLEVAL/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>Mr. O'Cruel is teaching Math to ninth grade students. Students of course are very lazy, so they do not like to do their homework. On the other side, Mr. O'Cruel doesn't like lazy students.Recently Andrew failed to do his homework again, so he was given a special task. If he doesn't do it, he will be expelled from his school. The task seems very easy, but it is very technical, so it would take a lot of time. Andrew is given a polynomial p(x) = anxn + an-1xn-1 + . . . + a1x + a0 with integer coefficients.</p>
<p>He must calculate the value of the polynomial for k successive integer numbers starting from l. Of course writing all these numbers would require too much paper. So as a proof of completing the task, for each number x from l to l + k - 1 Andrew is asked to provide the sum of squares of m last digits in decimal notation of p(x). Since Andrew is lazy, he doesn't want to do the task by himself. So he asks you to write the program that calculates the values requested.</p>
<h3>Input</h3>
<p>The first line of the input file contains n, l, k, and m (0 &lt;= n &lt;= 10, 0 &lt;= l &lt;= 10^1000 , 1 &lt;= k &lt;= 1 000, 1 &lt;= m &lt;= 1 000). The following n + 1 lines contain coefficients of the polynomial: an , an-1 , . . . , a1 , a0 (0 &lt;= ai &lt;= 10^1000).</p>
<pre>SAMPLE INPUT<br>3 0 10 2<br>1<br>0<br>2<br>1</pre>
<h3>Output</h3>
<p>Output k lines --- for x from l to l + k - 1 output the sum of squares of last m digits of p(x).</p>
<pre>SAMPLE OUTPUT<br>1<br>16<br>10<br>25<br>58<br>45<br>85<br>89<br>85<br>80</pre>
<p> </p>