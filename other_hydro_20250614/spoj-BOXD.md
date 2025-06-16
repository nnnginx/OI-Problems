<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>The University of Waterloo is famous for its booming population of geese, and many researchers go there to study them. One day, Doctor Y (known for his work in the field of boxology) decided to go there and investigate how good geese are at optimization problems.</p>
<p>At UW, there is a large lake (so large, in fact, that the boundaries are never an issue). Doctor Y decides to drop a number of 2D boxen onto this lake and command the geese to travel from one to another, recording how much time they spend flying as opposed to walking (naturally, the geese won��t swim, considering the not-so-appealing brown colour of the lake). He has a Boxdropper machine at his disposal to do the work for him �C he can give it the following commands:</p>
<p><strong>B </strong>$x_1$ $y_1$ $x_2$ $y_2$:&nbsp;Drop a box onto the lake such that its lower-left coordinate is at ($x_1$, $y_1$) and its upper-right coordinate is at ($x_2$, $y_2$). Doctor Y defines the origin to be somewhere in the middle of the lake. Note that boxen can overlap with one another.</p>
<p><strong>G </strong>$a$ $b$:&nbsp;Command the geese to travel from the <strong>a</strong><sup>th</sup> box dropped to the <strong>b</strong><sup>th</sup> one, and record the total distance that they fly.</p>
<p>Since the scientific community has not yet realized the benefits of studying boxen, Doctor Y isn��t receiving much funding �C as such, he only has $500$ boxen at his disposal, and his machine can only handle $10^6$ commands before it overheats.</p>
<p>The geese can walk across boxen freely, but sometimes they may have to fly over water to reach other boxen. The geese, secretly participating in the second stage of the Canadian Computing Competition every year, are well versed in optimization problems such as these, and so will always choose a path that will minimize the total distance that they spend flying. Given the commands that Doctor Y inputs into the Boxdropper, determine the distances recorded by it (one for every <strong>G</strong> command).</p>
<h3>Input</h3>
<p>On each line, one of the 2 types of commands will be given:</p>
<p>If the line starts with the character <strong>B</strong>, it will be followed by 4 integers ($x_1$, $y_1$, $x_2$, and $y_2$), each with absolute value no greater than $10^6$.</p>
<p>If the line starts with the character <strong>G</strong>, it will be followed by 2 integers ($a$ and $b$), with $a \neq b$&nbsp;and $1 \leq a,b \leq n$ (where $n$ is the number of <strong>B</strong> commands inputted so far).</p>
<p>Commands should be read until EOF.</p>
<h3>Output</h3>
<p>For every <strong>G</strong> command, output the distance that the geese spend flying. The numbers should be printed one per line, and rounded off to 2 decimal places.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">B -1 2 1 5</span>
<span style="font-family: 'courier new', courier;">B 3 -4 4 1</span>
<span style="font-family: 'courier new', courier;">G 2 1</span>
<span style="font-family: 'courier new', courier;">B 4 -3 6 -2</span>
<span style="font-family: 'courier new', courier;">B 6 -6 8 -4</span>
<span style="font-family: 'courier new', courier;">G 2 3</span>
<span style="font-family: 'courier new', courier;">G 1 4</span></pre>
<pre><strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">2.24</span>
<span style="font-family: 'courier new', courier;">0.00</span>
<span style="font-family: 'courier new', courier;">3.24</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>The lake looks like this:</p>
<p><img src="../../../content/sourspinach:boxdrop.bmp" alt="" width="275" height="325"></p>
<p>For the first <strong>G</strong> command, the geese must fly along the red line, which has a length of ��5.</p>
<p>For the second, the two boxen are touching, so no flight is necessary.</p>
<p>For the third, the geese must first fly along the red line, then walk across boxen 2 and 3, and finally fly along the blue line, which has a length of 1.</p>
<p>&nbsp;</p>