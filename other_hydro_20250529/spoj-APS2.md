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
<p>This problem is a harder version of <a href="../APS">APS</a>.</p>
<p>&nbsp;</p>
<p>Let $f(n)$ be the smallest prime factor of $n$. For example, $f(2) = 2,\ f(4) = 2$ and $f(35) = 5$.</p>
<p>The sequence $S(n)$ is defined for all positive integers as follows:</p>
<ul>
  <li>$S(1) = 0$</li>
  <li>$S(n) = S(n-1) + f(n)$ (if $n \ge 2$)</li>
</ul>
<p>Given $N$, find $S(N)$ <strong>modulo</strong> $2^{64}$.</p>
<h3>Input</h3>
<p>First line contains $T$ ($1 \le T \le 10000$), the number of test cases.</p>
<p>Each of the next $T$ lines contains a single integer $N$. ($1 \le N \le 1234567891011$)</p>
<h3>Output</h3>
<p>For each integer $N$, output a single line containing $S(N)$ <strong>modulo</strong> $2^{64}$.</p>
<h3>Example</h3>
<h4>Input</h4>
<pre>5<br>1<br>4<br>100<br>1000000<br>1000000000000</pre>
<h4>Output</h4>
<pre>0<br>7<br>1257<br>37568404989<br>7294954823202325427</pre>
<h3>Explanation for Input</h3>
<p>- $S(4) = 2 + 3 + 2 = 7$</p>
<p>- $S(10^{12}) = 18435592284459044389811 \equiv 7294954823202325427 \pmod{2^{64}}$</p>
<h3>Information</h3>
<p>There are 6 Input files.</p>
<p>- Input #0: $1 \le T \le 10000$, $1 \le N \le 10000$, TL = 1s.</p>
<p>- Input #1: $1 \le T \le 1000$, $1 \le N \le 10^{8}$, TL = 20s.</p>
<p>- Input #2: $1 \le T \le 200$, $1 \le N \le 10^{9}$, TL = 20s.</p>
<p>- Input #3: $1 \le T \le 40$, $1 \le N \le 10^{10}$, TL = 20s.</p>
<p>- Input #4: $1 \le T \le 7$, $1 \le N \le 10^{11}$, TL = 20s.</p>
<p>- Input #5: $T = 1$, $1 \le N \le 1234567891011$, TL = 20s.</p>
<p>My solution runs in 5.36 sec. (total time)</p>
<p><strong>Source Limit is 8 KB</strong>.</p>