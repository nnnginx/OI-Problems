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
<p>Let $(\ a_i\ )_{i=0}^\infty$ be the integer sequence such that: $$a_n =  \begin{cases} 0 &amp; (0 \le n &lt; k - 1) \\ 1 &amp; (n = k - 1)\\ b \cdot a_{n-j} + c \cdot a_{n-k} &amp; (n \ge k) \end{cases}, $$ where $j$, $k$, $b$ and $c$ is integer.</p>
<p>For each $n, j, k, b$ and $c$, find $a_n$ <strong>modulo</strong> $1\,000\,000\,037$.</p>
<h3>Input</h3>
<p>The first line contains $T$, the number of test cases.</p>
<p>Each of the next $T$ lines contains five integers $n, j, k, b$ and $c$.</p>
<h3>Output</h3>
<p>For each test case, print $a_n$ <strong>modulo</strong> $1\,000\,000\,037$.</p>
<h3>Constraints</h3>
<ul>
<li>$1 \le T \le 10^2$</li>
<li>$0 \le n \le 10^9$</li>
<li>$10^5 \le k \le 10^8$, $1 \le j &lt; k$</li>
<li>$1 \le b \le 10^9$, $1 \le c \le 10^9$</li>
</ul>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
1000000 1 100000 1 1
1000000000 1 100000000 1 1

<strong>Output:</strong>
372786243
994974348
</pre>