<p>Find the number of divisors of <strong><em>N</em></strong>! (factorial) very fast !</p>
<h3>Input</h3>
<p>The first line contains an integer <em><strong>T</strong></em>, the number of test cases.</p>
<p>Each line of the next <strong><em>T</em></strong> lines contains two integers <em><strong>N</strong></em> and <strong><em>M</em></strong>.</p>
<h3>Output</h3>
<p>For each line, output a single line containing the number of divisors of <strong><em>N</em></strong>! modulo <em><strong>M</strong></em>.</p>
<h3>Example</h3>
<h4>Input</h4>
<pre>3
10 989
10000 999989
10000000000 999999999989
</pre>
<h4>Output</h4>
<pre>270
616797
40946947081
</pre>
<h3>Constraints</h3>
<p>1 ¡Ü <strong><em>T</em></strong> ¡Ü 10<sup>4</sup><br> 0 ¡Ü <em><strong>N</strong></em> ¡Ü 10<sup>11</sup><br> 1 ¡Ü <em><strong>M</strong></em> ¡Ü 10<sup>12</sup></p>
<h3>Information</h3>
<p>There are 5 input files.</p>
<p>- Input #1: <strong><em>T</em></strong> ¡Ü 10<sup>4</sup>, <em><strong>N</strong></em> ¡Ü 10<sup>4</sup>, TL = 1s</p>
<p>- Input #2: <strong><em>T</em></strong> ¡Ü 5, <strong><em>N</em></strong> ¡Ü 10<sup>8</sup>, TL = 20s</p>
<p>- Input #3: <em><strong>T</strong></em> ¡Ü 5, <em><strong>N</strong></em> ¡Ü 10<sup>9</sup>, TL = 20s</p>
<p>- Input #4: <em><strong>T</strong></em> ¡Ü 5, <em><strong>N</strong></em> ¡Ü 10<sup>10</sup>, TL = 20s</p>
<p>- Input #5: <em><strong>T</strong></em> ¡Ü 5, <em><strong>N</strong></em> ¡Ü 10<sup>11</sup>, TL = 20s</p>
<p>My total running time is 3.14 sec. (C++)</p>
<h3>Credits</h3>
<ul>
<li><a href="../../../users/ravi_shank/">ivar.raknahs</a>&nbsp;-&nbsp;the original problem (<a href="../DIVFACT/">DIVFACT</a>) author</li>
<li><a href="../../../users/francky/">Francky</a>&nbsp;- the author of <a href="../DIVFACT2">DIVFACT2</a> and <a href="../DIVFACT3/">DIVFACT3</a></li>
</ul>