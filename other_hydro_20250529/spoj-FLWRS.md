<p>Hanadi has <strong>N</strong> flower pots each with a unique flower. The pots are&nbsp;arranged along in a line.</p>
<p>One day, She decided to change their&nbsp;order under the condition that no two pots that were</p>
<p>originally&nbsp;next to each other remain next to each other.</p>
<p>&nbsp;</p>
<h3 style="font-size: 1.17em;">Task</h3>
<p>write a program that is given the number of pots, calculates the&nbsp;number of possible orders</p>
<p>satisfying the condition&nbsp;<strong><span style="text-decoration: underline;">modulo a given integer M</span></strong>.</p>
<p>&nbsp;</p>
<h3 style="font-size: 1.17em;">Constraints</h3>
<p><strong>1</strong> ¡Ü <strong>N</strong> ¡Ü <strong>2,000</strong>&nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; The number of pots.</p>
<p><strong>2</strong> ¡Ü <strong>M</strong> ¡Ü <strong>1,000,000,000</strong></p>
<p><strong><br></strong></p>
<h3>Input</h3>
<ul>
<li>Line 1 contains the integer <strong>N</strong>, the number of flower pots.</li>
<li>Line 2 contains the integer <strong>M</strong>.</li>
</ul>
<h3>Output</h3>
<p>A single line containing one integer between <strong>0</strong> and <strong>M-1</strong> (inclusive):&nbsp;the number of possible</p>
<p>orders modulo <strong>M</strong>.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>5</pre>
<pre>11</pre>
<pre><strong>Output:</strong><br>3</pre>
<pre>For<strong> 5</strong> pots, there are <strong>14</strong> orders satisfying Hanadi's condition, assuming the original order</pre>
<pre>of pots was "<strong>ABCDE</strong>"</pre>
<pre>Then the <strong>14</strong> possible orders are:</pre>
<pre><p><strong>ACEBD</strong></p><p><strong>ADBEC</strong></p><p><strong>BDACE</strong></p><p><strong>BDAEC</strong></p><p><strong>BECAD</strong></p><p><strong>CADBE</strong></p><p><strong>CAEBD</strong></p><p><strong>CEADB</strong></p><p><strong>CEBDA</strong></p><p><strong>DACEB</strong></p><p><strong>DBEAC</strong></p><p><strong>DBECA</strong></p><p><strong>EBDAC</strong></p><p><strong>ECADB</strong></p><p><strong><br></strong></p><p><strong>14</strong> modulo <strong>11</strong> =<strong> 3</strong></p><p>So the answer is <strong>3</strong>.&nbsp;</p><p><strong><br></strong></p><p>&nbsp;</p></pre>
<ul>
<li>Number of test-cases is <strong>28</strong>.</li>
</ul>
<pre><br></pre>