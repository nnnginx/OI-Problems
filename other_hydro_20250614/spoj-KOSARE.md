<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Mirko found N boxes with various forgotten toys at his attic. There are M different toys, numbered 1&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">through M, but each of those can appear multiple times across various boxes.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Mirko decided that he will choose some boxes in a way that there is at least one toy of each kind</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">present, and throw the rest of the boxes away.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Determine the number of ways in which Mirko can do this.</div>
<p>&nbsp;</p>
<p>Mirko found N boxes with various forgotten toys at his attic. There are M different toys, numbered 1&nbsp;</p>
<p>through M, but each of those can appear multiple times across various boxes.</p>
<p>Mirko decided that he will <strong>choose some boxes</strong> in a way that there is <strong>at least one toy of each kind</strong></p>
<p>present, and throw the rest of the boxes away.</p>
<p>Determine the number of ways in which Mirko can do this.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>&nbsp;</p>
<p>The first line of input contains two integers N and M (1 ¡Ü N ¡Ü 1 000 000, 1 ¡Ü M ¡Ü 20).</p>
<p>Each of the following N lines contains an integer K<sub>i</sub>&nbsp;(0 ¡Ü K<sub>i</sub> ¡Ü M) followed by Ki distinct integers from&nbsp;</p>
<p>interval [1, M], representing the toys in that box.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>The first and only line of output should contain the requested number of ways modulo 1 000 000 007.</p>
<h3>Example</h3>
<pre><strong>Input 1:</strong>
3 3
3 1 2 3
3 1 2 3
3 1 2 3

<strong>Output 1:</strong>
7<span style="white-space: normal;">
</span></pre>
<pre><strong>Input 2:</strong>
3 3
1 1
1 2
1 3

<strong>Output 2:</strong>
1<span style="white-space: normal;">
</span></pre>
<pre><strong>Input 3:</strong>
4 5
2 2 3
2 1 2
4 1 2 3 5
4 1 2 4 5

<strong>Output 3:</strong>
6<span style="white-space: normal;">
</span></pre>