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
<p>This problem is a harder version of <a href="../TRENDGCD/">TRENDGCD</a>.</p>
<p>Given $n$ and $m$, compute</p>
<p>$$ S(n, m) = \sum_{i=1}^n \sum_{j=1}^m ij \cdot f(\gcd(i,j)), $$</p>
<p>where $f(n) = (\mu(n))^2 n$ and $\mu(n)$ is the Möbius function, that is, $f(n) = n$ if $n$ is square-free and $0$ otherwise. Especially, $f(1)=1$.</p>
<h3>Input</h3>
<p>The first line contains an integer $T$, indicating the number of test cases.</p>
<p>Each of the next $T$ lines contains two positive integers $n$ and $m$.&nbsp;</p>
<h3>Output</h3>
<p>For each test case, print $S(n, m)$ modulo $10^9+7$ in a single line.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5<br>42 18<br>35 1<br>20 25<br>123456789 987654321<br>233333333333 233333333333

<strong>Output:</strong>
306395<br>630<br>128819<br>897063534<br>355737203</pre>
<h3>Constraints</h3>
<p>There are 6 test files.</p>
<p>Test #0: $1 \leq T \leq 10000$, $1 \leq n, m \leq 10^7$.</p>
<p>Test #1: $1 \leq T \leq 200$, $1 \leq n, m \leq 10^8$.</p>
<p>Test #2: $1 \leq T \leq 40$, $1 \leq n, m \leq 10^9$.</p>
<p>Test #3: $1 \leq T \leq 10$, $1 \leq n, m \leq 10^{10}$.</p>
<p>Test #4: $1 \leq T \leq 2$, $1 \leq n, m \leq 10^{11}$.</p>
<p>Test #5: $T = 1$, $1 \leq n, m \leq 235711131719$.</p>
<p>@Speed Addicts: My solution runs in 20.76s (total time). (approx 3.46s per file)</p>
<p><strong>WARNING</strong>: The time limit may be somewhat strict.</p>