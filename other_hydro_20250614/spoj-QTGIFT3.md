<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/QTGIFT3/en/">English</a></td>
<td width="50%"><a href="/problems/QTGIFT3/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p> </p>
<p>Christmas will come next month, so DB is planning to give TN a wonderful gift.</p>
<p>The city that DB and TN are living has n intersections. Each direct connections between 2 intersections has its length. In the Chirstmas night, TN will wait at the t-th intersection, and DB will start from the s-th intersection go throught some connections, to the date place.</p>
<p>Of course DB doesn¡¯t want to make TN wait for long time, so he will choose the shortest path. He also want to know how many different shortest paths from s to t (there is at least one path).</p>
<p>Because the number of intersections and connections are too large, DB can¡¯t calculate these himself, so he need you help.</p>
<h3>Input</h3>
<p>-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; First line : 3 positive integers, n, s and t (2 ¡Ü n ¡Ü 10<sup>5</sup>, 1 ¡Ü s, t ¡Ü n, s ¡Ù t)</p>
<p>-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; n lines : the i-th line contains 3 positive integers l, r, w, means there are direct connections from i to l, i to l + 1, ¡­ i to r, each has length w (1 ¡Ü l ¡Ü r ¡Ü n, w ¡Ü 10<sup>6</sup>)</p>
<h3>Output</h3>
<p>-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Two positive integers, length of the shortest path, and number of the shortest paths (modulo 10<sup>15</sup>), separate by a space</p>
<h3>Example</h3>
<p>&nbsp;</p>
<pre><img style="float: right;" src="../../../content/kata69:QTGIFT3.bmp" alt="QTGIFT3_Graph" width="350" height="228"></pre>
<pre><strong>Input:</strong></pre>
<pre><strong><span style="white-space: pre;">	</span>4 1 4</strong></pre>
<pre><strong><span style="white-space: pre;">	</span>2 3 3</strong></pre>
<pre><strong><span style="white-space: pre;">	</span>3 4 5</strong></pre>
<pre><strong><span style="white-space: pre;">	</span>2 4 5</strong></pre>
<pre><strong><span style="white-space: pre;">	</span>1 2 6<strong><br></strong></strong>
<strong>Output:</strong>
<span style="white-space: pre;">	</span><strong>8 2</strong>
</pre>
<pre><p><span style="white-space: pre;">	</span></p><p><strong>Detais : </strong>Two shortest paths are : (1, 2, 4) and (1, 3, 4)			</p></pre>
<p></p>