<p>This day (7 February 2013) is my 19th birthday <img title="Laughing" src="../../../gfx/jscripts/tiny_mce/plugins/emotions/img/smiley-laughing.gif" border="0" alt="Laughing">&nbsp;So, I want to celebrate&nbsp;it on SPOJ by making this EASY puzzle problem.</p>
<p>This game/puzzle is about matches, given <strong>n</strong> matches, your task is to arrange the matches (not necessarily all) such that number of rectangle (any size) is maximum.</p>
<h3>Input</h3>
<p>First line there is an integer <strong>T</strong><span style="color: #222222; font-family: arial, sans-serif; font-size: small; line-height: 16px;">¡Ü</span>100 then <strong>T</strong> lines follow, each line contain an integer <strong>n</strong>&lt;1.000.000.000.</p>
<h3>Output</h3>
<p>For each test case, output required answer (maximum number of rectangles)</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre>5</pre>
<pre>3</pre>
<pre>4</pre>
<pre>8</pre>
<pre>12</pre>
<pre>15</pre>
<pre><strong>Output:</strong></pre>
<pre>0</pre>
<pre>1</pre>
<pre>3</pre>
<pre>9</pre>
<pre>12</pre>
<h3>Explanation</h3>
<p>--&gt;First test case: No rectangle can be formed with only 3 matches</p>
<p>--&gt;Second test case: Only one rectangle can be formed with 4 mathes</p>
<p>--&gt;Third test case:</p>
<p><span style="white-space:pre"> </span>there are max 3 rectangles (2 size 1x1, 1 size 2x1) can be formed with number of matches&lt;=8, here is one of the mathes formation:</p>
<p><span style="white-space:pre"> </span><img title="Case 3" src="file://3zkoAx8D.png" alt="Case 3" width="251" height="133"></p>
<p>--&gt;Fourth test case:</p>
<p><span style="white-space:pre"> </span>there are max 9 rectangles (4 size 1x1, 2 size 2x1, 2 size 1x2, 1 size 2x2) can be formed with number of matches &lt;=12, here is one of the formation:</p>
<p><span style="white-space:pre"> </span><img title="case 4" src="file://jpgs9RiG.png" alt="case 4" width="250" height="254"></p>
<p>--&gt;Fifth test case:</p>
<p><span style="white-space:pre"> </span>there are max 12 rectangles (5 size 1x1, 3 size 2x1, 1 size 3x1, 2 size 1x2, 1 size 2x2) can be formed with number of matches &lt;=15, here is one of the formation:</p>
<p><span style="white-space:pre"> </span><img title="case 5" src="file://aPbQTcfH.png" alt="case 5" width="371" height="256"></p>
<h3>Information</h3>
<p>Time limit¡Ö150x my program speed, Enjoy this birthday party game, I set this problem such that semi naive solution will pass..</p>
<p><strong>See also:</strong> <a title="TJANDRA" href="../TJANDRA/" target="_blank">Another problem added by Tjandra Satria Gunawan</a></p>