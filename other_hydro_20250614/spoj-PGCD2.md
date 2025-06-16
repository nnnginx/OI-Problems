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
<p>This problem is a harder version of <a href="../PGCD/">PGCD</a>.</p>
<p>Let $P$ be the set of all prime numbers. For two positive integers $n$ and $m$, define</p>
<p>$$ f(n,m) = \sum_{i=1}^n \sum_{j=1}^m [\gcd(i,j) \in P], $$</p>
<p>which counts the number of prime numbers among the greatest common divisors $\gcd(i,j)$ for $1 \leq i \leq n$ and $1 \leq j \leq m$.</p>
<p>Your task: given $n$ and $m$, compute $f(n,m)$.</p>
<h3>Input</h3>
<p>The first line contains an integer $T$, indicating the number of test cases.</p>
<p>Each of the next $T$ lines contains two positive integers $n$ and $m$.&nbsp;</p>
<h3>Output</h3>
<p>For each test case, print $f(n, m)$ in a single line.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4<br>10 10<br>100 100<br>123456789 987654321<br>233333333333 233333333333

<strong>Output:</strong>
30<br>2791<br>33523360713808196<br>14968599673221238693021</pre>
<h3>Constraints</h3>
<p>There are 6 test files.</p>
<p>Test #0: $1 \leq T \leq 10000$, $1 \leq n, m \leq 10^7$.</p>
<p>Test #1: $1 \leq T \leq 200$, $1 \leq n, m \leq 10^8$.</p>
<p>Test #2: $1 \leq T \leq 40$, $1 \leq n, m \leq 10^9$.</p>
<p>Test #3: $1 \leq T \leq 10$, $1 \leq n, m \leq 10^{10}$.</p>
<p>Test #4: $1 \leq T \leq 2$, $1 \leq n, m \leq 10^{11}$.</p>
<p>Test #5: $T = 1$, $1 \leq n, m \leq 235711131719$.</p>
<p>@Speed Addicts: My solution runs in 4.87s (total time). (approx 0.81s per file)</p>