<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.7.1/katex.min.css" integrity="sha384-wITovz90syo1dJWVh32uuETPVEtGigN07tkttEqPv+uR2SE/mbQcG7ATL28aI9H0" crossorigin="anonymous">
<script src="https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.7.1/katex.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.7.1/contrib/auto-render.min.js"></script>
<script type="text/javascript">// <![CDATA[
document.addEventListener("DOMContentLoaded", function(){
  renderMathInElement(
    document.body,{
      delimiters: [
        {left: "$$", right: "$$", display: true},
        {left: "$", right: "$", display: false}]})});
// ]]></script>

<p>Let $\sigma_0(n)$ be the number of positive divisors of $n$.</p>
<p>For example, $\sigma_0(1) = 1$, $\sigma_0(2) = 2$ and $\sigma_0(6) = 4$.</p>
<p>Let $$S_k(n) = \sum _{i=1}^n \sigma_0(i^k).$$</p>
<p>Given $n$ and $k$, find $S_k(n) \bmod 2^{64}$.</p>
<h3>Input</h3>
<p>There are multiple test cases. The first line of input contains an integer $T$ ($1 \le T \le 10000$), indicating the number of test cases. For each test case:</p>
<p>The first line contains two integers $n$ and $k$ ($1 \le n, k \le 10^{10}$).</p>
<h3>Output</h3>
<p>For each test case, output a single line containing $S_k(n) \bmod 2^{64}$.</p>
<h3>Example</h3>
<h4>Input</h4>
<pre>5
1 3
2 3
3 3
10 3
100 3
</pre>
<h4>Output</h4>
<pre>1
5
9
73
2302
</pre>
<h3>Information</h3>
<p>There are 5 Input files.</p>
<ul>
<li>Input #1: $1 \le n \le 10000$, TL = 1s.</li>
<li>Input #2: $1 \le T \le 300,\ 1 \le n \le 10^7$, TL = 5s.</li>
<li>Input #3: $1 \le T \le 75,\ 1 \le n \le 10^{8}$, TL = 5s.</li>
<li>Input #4: $1 \le T \le 15,\ 1 \le n \le 10^{9}$, TL = 5s.</li>
<li>Input #5: $1 \le T \le 5,\ 1 \le n \le 10^{10}$ , TL = 5s.</li>
</ul>
<p>My C++ solution runs in 5.6 sec. (total time)</p>
<h3>Notes</h3>
<p>This is general version of <a href="../DIVCNT1">DIVCNT1</a>, <a href="../DIVCNT2">DIVCNT2</a> and <a href="../DIVCNT3">DIVCNT3</a>. You may want to solve these three problems first.</p>