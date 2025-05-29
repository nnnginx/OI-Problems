<p>You are given N <span style="color: #ff0000;"><strong>different </strong></span>circles , while some region may be covered more than once.</p>
<p>If one region is covered by K times, then it was called a "K- Region".</p>
<p>So, you are expected to output the area of all the regions! (K from 1 to N)</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line is one integer n indicates the number of the circles.  (1 &lt;= n &lt;= 1000)</p>
<p>Then follows n lines every line has three integers</p>
<p>Xi Yi Ri</p>
<p>indicates the coordinate of the center of the circle, and the radius.  (|Xi|. |Yi|&nbsp; &lt;= 1000, 0 &lt; Ri &lt;= 1000)</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>Output N lines, the i-th line output</p>
<p>[i] = area_of_i_region</p>
<p>here the area must round to&nbsp; 3 digits after decimal point.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3<br>0 0 1<br>1 0 1<br>1 1 1<br><br><strong>Output:</strong>
[1] = 4.699<br>[2] = 1.699<br>[3] = 0.443<br></pre>