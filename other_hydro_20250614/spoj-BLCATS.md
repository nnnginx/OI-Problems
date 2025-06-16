<p>There is a circle of n cats, includes white cats, red cats and green cats. When two cats of different colors talk with each other, they both change to third color. If they have same color, nothing will happen.</p>
<p>At each step, the 1<sup>st</sup>&nbsp;cat talks with 2<sup>nd</sup>&nbsp;cat, the 2<sup>nd</sup>&nbsp;cat talks with the 3<sup>rd</sup>&nbsp;cat,¡­ and the n<sup>th</sup>&nbsp;cat talks with 1<sup>st</sup>&nbsp;cat.</p>
<p>Given the original color of n cats, your task is find the color of n cats after k steps.</p>
<h3>Input</h3>
<p>-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; First line : n and k (1 ¡Ü n ¡Ü 50000, 1 ¡Ü k ¡Ü 10<sup>9</sup>)</p>
<p>-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Second line : n characters, the i-th charater denotes color of the i-th cat at first state</p>
<h3>Output</h3>
<p>-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; n charaters denotes the color of n cats after k steps.</p>
<h3>Example</h3>
<pre><p>Input :</p><p><span style="white-space: pre;">	</span>3 1</p><p><span style="white-space: pre;">	</span>GRR</p><p>Output :</p><p><span style="white-space: pre;">	</span>RGR</p></pre>
<p>&nbsp;</p>
<pre><p>Input :</p>
<p><span style="white-space: pre;">	</span>5 4</p><p><span style="white-space: pre;">	</span>WRWRW</p><p>Output :</p><p><span style="white-space: pre;">&nbsp;<span style="white-space: pre;">	</span></span>GGGWG</p></pre>
<p><strong>Note :</strong> Before solving this problem, you may want to try&nbsp;<a href="../COLORCAT" target="_blank">COLORCAT</a></p>