<p>In a galaxy far far away there is a new low-cost space carrier starting daily&nbsp;interplanetary flights.<br>In the galaxy there are&nbsp;<strong>N</strong> planets, numbered with integers from 1 to <strong>N</strong>. Cost of a flight between two planets&nbsp;<br>depends only on take-off/landing fees of those planets. For each planet <strong>k</strong> you are given his fee, <strong>p<sub>k</sub></strong>, so the cost<br>of a flight between planets <strong>a</strong> and <strong>b</strong> is <strong>p<sub>a</sub> + p<sub>b</sub></strong>.&nbsp;</p>
<p>Space carrier wants to determine the flights it will offer daily so that any planet can be reached from any other planet, directly or indirectly.</p>
<p>Because of space reasons it's possible to conduct flights only between certain pairs of planets.<br>Allowed flights are described with <strong>M</strong> permissions of form "<strong>x<sub>k</sub> a<sub>k</sub> b<sub>k</sub></strong>" which means it's possible to conduct a bidirectional flight&nbsp;between planet <strong>x<sub>k</sub></strong> and any planet <strong>c</strong>, where <strong>a<sub>k</sub></strong>&nbsp;¡Ü&nbsp;<strong>c</strong>&nbsp;¡Ü&nbsp;<strong>b<sub>k</sub></strong>.</p>
<p>Find the minimum total cost of offered flights such that all planets are connected.</p>
<h3>Input</h3>
<p>N M<br>p<sub>1</sub> p<sub>2</sub> .. p<sub>N</sub>&nbsp;<br>x<sub>1</sub> a<sub>1</sub> b<sub>1<br></sub>x<sub>2</sub> a<sub>2</sub> b<sub>2</sub><br>..<br>x<sub>M</sub> a<sub>M</sub> b<sub>M</sub>&nbsp;</p>
<p>1 ¡Ü N, M ¡Ü 10<sup>5</sup><br>For each p<sub>k</sub> following holds: 0 ¡Ü p<sub>k</sub> ¡Ü 10<sup>6</sup>.<br>For each permission it holds that either x<sub>k</sub> &lt; a<sub>k</sub> or x<sub>k</sub> &gt; b<sub>k</sub>.<br>Also, it's possible that some pairs of planets are listed in more than one permission.&nbsp;</p>
<p>It will always be possible to choose flights such that all planets are connected.</p>
<h3>Output</h3>
<p>Minimum daily cost of space carrier transportation system.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
6 8<br>3 5 8 2 9 4 <br>3 1 2 <br>6 3 3 <br>3 1 1 <br>6 2 2 <br>2 3 6 <br>3 1 2 <br>3 2 2 <br>4 1 1

<strong>Output:</strong>
46</pre>
<pre>Explanation: we connect following pairs of planets: (1, 3), (1, 4), (4, 2), (2, 5), (2, 6).</pre>