<p>There are M modern washbasins numbered from 1 to M from left to right in the ladies’ room of an enormous shopping centre.</p>
<p>Currently, there are N ladies in the restroom (numbered from 1 to N) and they’ve occupied the washbasins with numbers A<sub>1</sub>, A<sub>2</sub>, . . . , A<sub>N</sub> . Soon there will be M − N more ladies arriving (numbered from N + 1 to M in the order of arrival) that will occupy all the remaining available washbasins.</p>
<p>The ladies arriving primarily want their privacy, so each of them always chooses an available washbasin by the following procedure:</p>
<p><span style="white-space:pre"> </span>• First she finds the largest consecutive series of available washbasins. If there is more than one, she chooses the leftmost.<br><span style="white-space:pre"> </span>• After that, she occupies the middle washbasin in the chosen series. If the series is of even length, she chooses the left of the two middle washbasins.</p>
<p>It is safe to assume that none of the ladies will leave the washbasin in the foreseeable future.</p>
<p>Write a programme that will, for each of Q given integers B<sub>i</sub> , determine the label of the washbasin that will be occupied by the lady marked with B<sub>i</sub>.</p>
<h3>Input</h3>
<p>The first line of input contains integers M, N and Q – the number of washbasins, the initial number of ladies in the restroom and the number of ladies for which you need to determine which washbasin they will use.</p>
<p>The second line of input contains N space-separated integers, the i th of those numbers is A<sub>i</sub> – the label of the washbasin that is being used by lady i.</p>
<p>The third line of input contains Q space-separated integers, the i th of those numbers is B<sub>i</sub> – the label of the lady for which we want to know which washbasin she will use.</p>
<p>The first N ladies in the restroom haven’t necessarily chosen their washbasins using the procedure described in the task.</p>
<p>The arrays A and B are strictly increasing. In other words, it holds 1 &lt;= A<sub>1</sub> &lt; A<sub>2</sub> &lt; . . . &lt; A<sub>N</sub> &lt;= M and 1 &lt;= B<sub>1</sub> &lt; B<sub>2</sub> &lt; . . . &lt; B<sub>Q</sub> &lt;= M.</p>
<h3>Output</h3>
<p>Output Q lines. The i th line must contain the label of the washbasin that will be used by the lady labeled B<sub>i</sub> .</p>
<p><span style="font-size: 1.17em;"><strong>Constraints</strong></span></p>
<p><span style="font-size: 1.17em;">&nbsp;</span>1 &lt;= N &lt;= M &lt;= 10^14<br>1 &lt;= Q, N &lt;= 10^5</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
7 1 4&nbsp;<br>4&nbsp;<br>2 3 4 5</pre>
<pre><strong>Output:</strong>
2 <br>6 <br>1 <br>3<br><span style="font-weight: bold;"><br></span></pre>
<pre><span style="font-weight: bold;">Input:<br></span>10 2 4&nbsp;<br>2 8 <br>1 3 5 8</pre>
<pre><strong>Output:<br></strong>2<br>5<br>6<br>4</pre>
<pre><strong>Clarification of the second example:</strong> <br>The first two ladies occupy the washbasins 2 and 8 (respectively). <br>The remaining ladies occupy the washbasins 5, 3, 6, 9, 1, 4, 7 and 10, respectively.</pre>
<pre><strong><br></strong></pre>
<pre><strong>Source: </strong>Croatian Olympiad in Informatics 2015 </pre>