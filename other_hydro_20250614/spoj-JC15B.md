<p><span style="font-size: x-large;"><strong>Folding Stick</strong></span></p>
<p><img src="../../../content/tjandra:X_cover.png" alt="" width="456" height="300"></p>
<p>Today Satria really excited about fractals (recurrence pattern), the first fractal type he learn is the dragon curve fractal. To make the dragon curve, it can be easily simulated by folding the paper and open it 90 degrees (parellel to X axis or Y axis) like this image below:</p>
<p><img src="../../../content/tjandra:fold.jpg" alt="" width="600" height="140"></p>
<p>Satria realized that the can be many ways to fold the paper, so he make an experiment. Initially there is a stick length 2<sup>N</sup>, he then place the stick parallel to x axis with one end lies on coordinate (0,0) and the other end lies on coordinate (2<sup>N</sup>,0). He then fold the stick, so the new folded stick occupy (0,0) to (2<sup>N-1</sup>,0) he keep doing that until the final folded stick occupy (0,0) to (1,0). In each foding there are two types of folding, folding UP (via possitive Y coordinate) and folding down (via negative Y coordinate). he then open all the folding with angle 90 degrees so each stick segment will be parallel ot X axis or Y axis. Now he wonder if he open all the folding with angle 90 degrees, what is the coordinate of the other end of that stick. Can you help him?</p>
<p><span style="font-size: large;"><strong>Input</strong></span></p>
<p>The first line there is an integer N denoting number of folding and a string S the sequence of folding and the type of folding.</p>
<p><strong><span style="font-size: large;">Output</span></strong></p>
<p>You sould output two integers x and y which is the coordinate of the other end of that stick.</p>
<ul>
</ul>
<p><strong><span style="font-size: large;">Constraint</span></strong></p>
<p>1 ¡Ü N ¡Ü 50</p>
<p>Length of string S is equal to N, in other word: |S|=N.</p>
<p>String S containing two possible characters:</p>
<ul>
<li>'U' means folding UP (positive Y direction)</li>
<li>'D' means folding DOWN (negative Y direction)</li>
</ul>
<p><strong><span style="font-size: large;">Sample 1</span></strong></p>
<p><span style="text-decoration: underline;">Input</span></p>
<pre>1 U</pre>
<p><span style="text-decoration: underline;">Output</span></p>
<pre>1 1</pre>
<p><strong><span style="font-size: large;">Sample 2</span></strong></p>
<p><span style="text-decoration: underline;">Input</span></p>
<pre>1 D</pre>
<p><span style="text-decoration: underline;">Output</span></p>
<pre>1 -1</pre>
<p><strong><span style="font-size: large;">Sample 3</span></strong></p>
<p><span style="text-decoration: underline;">Input</span></p>
<pre>2 UD</pre>
<p><span style="text-decoration: underline;">Output</span></p>
<pre>2 0</pre>
<p><strong><span style="font-size: large;">Sample 4</span></strong></p>
<p><span style="text-decoration: underline;">Input</span></p>
<pre>2 DU</pre>
<p><span style="text-decoration: underline;">Output</span></p>
<pre>2 0</pre>
<p><strong><span style="font-size: large;">Sample 5</span></strong></p>
<p><span style="text-decoration: underline;">Input</span></p>
<pre>3 UUU</pre>
<p><span style="text-decoration: underline;">Output</span></p>
<pre>-2 2</pre>
<p><strong><span style="font-size: large;">Sample 3 Explanation</span></strong></p>
<p>Here is the image illustrating sample 3 on how the stick is folded and openned with 90 degrees angle.&nbsp;</p>
<p><img src="../../../content/tjandra:X_explain_2.png" alt=""></p>
<p>As seen in the picture above the other end of the stick after folding and openning lies on coordinate (2,0).</p>
<p><strong><span style="font-size: large;">Sample 5 explanation</span></strong></p>
<p>Here is the final openned stick on test case 5, the other end of the stick after folding and openning lies on coordinate (-2,2)</p>
<p><img src="../../../content/tjandra:X_explain_1.png" alt=""></p>