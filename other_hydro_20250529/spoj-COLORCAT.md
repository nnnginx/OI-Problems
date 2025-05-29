<p>There is a circle with n cats, includes white cats, red cats and green cats. When two cats with different color talk with each other, they both change to third color. If they are same color, nothing will happen.</p>
<p>At each step, the 1<sup>st</sup> cat talks with 2<sup>nd</sup> cat, the 2<sup>nd</sup> cat talks with the 3<sup>rd</sup> cat,¡­ and the n<sup>th</sup> cat talks with 1<sup>st</sup> cat.</p>
<p>Given the original color of n cats, your task is find the color of n cats after k steps.</p>
<p><strong>Input :</strong></p>
<p>-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; First line : n and k (1 ¡Ü n ¡Ü 20000, 1 ¡Ü k ¡Ü 30000)</p>
<p>-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Second line : n characters, the i-th charater denotes color of the i-th cat at first state</p>
<p><strong>Output :</strong></p>
<p>-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; n charaters denotes the color of n cats after k steps.</p>
<p><strong>Sample :</strong></p>
<p>Input :</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 3 1</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; GRR</p>
<p>Output :</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; RGR</p>
<p>Input :</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 5 4</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; WRWRW</p>
<p>Output :</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; GGGWG</p>
<p>&nbsp;</p>
<p><strong>Note :</strong> After solved this problem, you may want to try&nbsp;<a href="../BLCATS" target="_blank">BLCATS</a></p>