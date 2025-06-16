<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.7.1/katex.min.css" integrity="sha384-wITovz90syo1dJWVh32uuETPVEtGigN07tkttEqPv+uR2SE/mbQcG7ATL28aI9H0" crossorigin="anonymous">
<script src="https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.7.1/katex.min.js" integrity="sha384-/y1Nn9+QQAipbNQWU65krzJralCnuOasHncUFXGkdwntGeSvQicrYkiUBwsgUqc1" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.7.1/contrib/auto-render.min.js"></script>
<script>// <![CDATA[
document.addEventListener("DOMContentLoaded", function(){
  renderMathInElement(
    document.body,{
      delimiters: [
        {left: "$$", right: "$$", display: true},
        {left: "$", right: "$", display: false}]})});
// ]]></script>
<p>Let $s_1(n)$ be the sum of positive <strong>proper</strong> divisors of $n$.</p>
<p>For example, $s_1(1) = 0$, $s_1(2) = 1$ and $s_1(6) = 6$.</p>
<p>Let $$S(n) = \sum _{i=1}^n s_1(i).$$</p>
<p>Given $N$, find $S(N)$.</p>
<h3>Input</h3>
<p>First line contains $T$&nbsp;($1 \le T \le 10^5$), the number of test cases.</p>
<p>Each of the next $T$ lines contains a single integer $N$. ($1 \le N &lt; 2^{63}$)</p>
<h3>Output</h3>
<p>For each number $N$, output a single line containing $S(N)$.</p>
<h3>Example</h3>
<h4>Input</h4>
<pre>6
1
2
3
10
100
1000000000000000000
</pre>
<h4>Output</h4>
<pre>0
1
2
32
3249
322467033424113218863487627735401433
</pre>
<h3>Information</h3>
<p>There are 6 Input files.</p>
<p>- Input #1: $1 \le N \le 10^5$, TL = 2s.</p>
<p>- Input #2: $1 \le T \le 60,\ 1 \le N \le 10^{15}$, TL = 10s.</p>
<p>- Input #3: $1 \le T \le 25,\ 1 \le N \le 10^{16}$, TL = 10s.</p>
<p>- Input #4: $1 \le T \le 10,\ 1 \le N \le 10^{17}$, TL = 10s.</p>
<p>- Input #5: $1 \le T \le 5,\ 1 \le N \le 10^{18}$, TL = 10s.</p>
<p>- Input #6: $1 \le T \le 2,\ 1 \le N &lt; 2^{63}$, TL = 10s.</p>
<p>My C++ solution runs in about 0.85 seconds for each Input #2 - #6.</p>
<h3>Note</h3>
<ul>
<li>Probably, $O(\sqrt{n})$ solutions will not pass.</li>
<li>Intended solutions have a running time of about $O(n^{1/3} \log n)$.</li>
<li>Time limits are somewhat <strong>strict</strong>.</li>
<li>The answer can be $\ge 2^{64}$.</li>
<li><a href="../DIVCNT1">DIVCNT1</a> is a little easier than this.</li>
</ul>