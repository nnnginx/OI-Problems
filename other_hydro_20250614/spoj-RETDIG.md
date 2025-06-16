<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>The adventures of ※Digger§ continue as he once again searches for treasure. This time, his money senses detect it underground. His plan is to dig down to it using an automatic pickaxe and his souped-up pneumatic drill.</p>
<p>The treasure is within a thin stretch of land, running West to East, that is made up of dirt and some rocks. This stretch is $L$ ($1 \leq L \leq 200$) metres long. Digger＊s money senses are very exact, and he knows the location of the treasure he seeks 每 it is no more than $10000$ metres below the surface. In addition to money senses, he apparently also has rock senses, which can pinpoint $N$ ($1 \leq N \leq 5000$) rocks among the dirt, none of which will be at a depth of more than $10000$ metres.</p>
<p>Digger＊s specially-designed pneumatic drill can only go straight down, and it can tunnel through dirt easily 每 however, it isn＊t equipped with brakes, so it keeps on going until it hits a rock. When this happens, it stops just above the rock, but the drill bit also breaks. This time, Digger doesn＊t have to worry about fuel 每 instead, he just wants to avoid breaking his drill bits! Once stationary, Digger can also use his pickaxe to dig left and right (yes, even through rocks!), but he can＊t dig up or down with it.</p>
<p>The treasure is pretty fragile, so Digger definitely doesn＊t want to drill right into it. Instead, he can either get to the same depth as it and use his pickaxe to dig to it, or he can use his pneumatic drill to go right past it (either 1 metre to the left or right of it). However, once he gets his hands on the treasure, Digger＊s plan isn＊t complete 每 he intends to keep drilling down until he gets to China. As such, he must first navigate past the deepest of the $N$ rocks 每 at that point, it＊s all dirt (or so he hopes...).</p>
<p>Digger can start anywhere on the surface. Determine the minimum amount of drill bits that he must break in order to retrieve the treasure and dig down past all the rocks, if it＊s possible at all.</p>
<h3>Input</h3>
<p>Line $1$: $L$ and $N$ 每 respectively, the length of the stretch of land (in metres) and the number of rocks.</p>
<p>Lines $2..N+1$: $A$ and $B$ 每 the $i$th line gives the location of the ($i-1$)th rock, where $A$ is its depth, and $B$ is its distance from the West edge of the stretch of land (both in metres).</p>
<p>Line $N+2$: $Y$ and $X$ 每 the location of the treasure, where $Y$ is its depth, and $X$ is its distance from the West edge of the stretch of land (both in metres). The treasure will not be within a rock.</p>
<h3>Output</h3>
<p>If it＊s impossible for Digger to reach the treasure and dig down past all the rocks, output ※Use dynamite§.</p>
<p>Otherwise, output a single number 每 the minimum number of drill bits Digger must break to accomplish this.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">10 20</span>
<span style="font-family: 'courier new', courier;">1 5</span>
<span style="font-family: 'courier new', courier;">2 1</span>
<span style="font-family: 'courier new', courier;">2 2</span>
<span style="font-family: 'courier new', courier;">2 4</span>
<span style="font-family: 'courier new', courier;">2 5</span>
<span style="font-family: 'courier new', courier;">2 6</span>
<span style="font-family: 'courier new', courier;">2 8</span>
<span style="font-family: 'courier new', courier;">2 9</span>
<span style="font-family: 'courier new', courier;">3 3</span>
<span style="font-family: 'courier new', courier;">4 7</span>
<span style="font-family: 'courier new', courier;">4 8</span>
<span style="font-family: 'courier new', courier;">4 9</span>
<span style="font-family: 'courier new', courier;">5 3</span>
<span style="font-family: 'courier new', courier;">5 4</span>
<span style="font-family: 'courier new', courier;">5 5</span>
<span style="font-family: 'courier new', courier;">5 6</span>
<span style="font-family: 'courier new', courier;">6 3</span>
<span style="font-family: 'courier new', courier;">10 1</span>
<span style="font-family: 'courier new', courier;">10 2</span>
<span style="font-family: 'courier new', courier;">10 7</span>
<span style="font-family: 'courier new', courier;">8 6</span></pre>
<pre><strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">3</span></pre>
<pre><span style="font-weight: bold;">Explanation of Sample:</span></pre>
<p>Digger starts on the surface, 7 metres from the West edge of the stretch of land. He drills down for 3 metres until he hits a rock and breaks his first drill bit. He then uses his pickaxe to walk to the left, and drills down another metre, hitting another rock and breaking his second drill bit. He then walks to the right (through a rock), and drills down for 5 metres, picking up the treasure on the way, until he hits another rock and breaks his third and final drill bit. He then walks to the right and drills down past the last rock. This route is shown below (＆.＊: dirt, ＆x＊: rock, ＆T＊: treasure, ＆D＊: drill, ＊&lt;＊ or ＆&gt;＊: pickaxe):</p>
<pre><span style="font-family: 'courier new', courier;">.....x.D..</span>
<span style="font-family: 'courier new', courier;">.xx.xxxDxx</span>
<span style="font-family: 'courier new', courier;">...x..&lt;D..</span>
<span style="font-family: 'courier new', courier;">......D&gt;xx</span>
<span style="font-family: 'courier new', courier;">...xxxxD..</span>
<span style="font-family: 'courier new', courier;">...x...D..</span>
<span style="font-family: 'courier new', courier;">.......D..</span>
<span style="font-family: 'courier new', courier;">......TD..</span>
<span style="font-family: 'courier new', courier;">.......D&gt;.</span>
<span style="font-family: 'courier new', courier;">.xx....xD.</span>
<span style="font-family: 'courier new', courier;">........D.</span></pre>
<p>&nbsp;</p>