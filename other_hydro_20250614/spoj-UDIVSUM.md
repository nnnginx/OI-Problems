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

<p>A natural number $d$ is a unitary divisor of $n$ if $d$ is a divisor of $n$ and if $d$ and $\frac{n}{d}$ are coprime.</p>
<p>Let $\sigma^{*}(n)$ be the sum of the unitary divisors of $n$. For example, $\sigma^{*}(1) = 1$, $\sigma^{*}(2) = 3$ and $\sigma^{*}(6) = 12$.</p>
<p>Let $$S(n) = \sum_{i=1}^n \sigma^{*}(i).$$</p>
<p>Given $n$, find $S(n) \bmod 2^{64}$.</p>
<h3>Input</h3>
<p>There are multiple test cases. The first line of input contains an integer $T$ ($1 \le T \le 50000$), indicating the number of test cases. For each test case:</p>
<p>The first line contains an integer $n$ ($1 \le n \le 5 \times 10^{13}$).</p>
<h3>Output</h3>
<p>For each test case, output a single line containing $S(n) \bmod 2^{64}$.</p>
<h3>Example</h3>
<h4>Input:</h4>
<pre>7
1
2
3
4
5
100
100000
</pre>
<h4>Output:</h4>
<pre>1
4
8
13
19
6889
6842185909
</pre>
<h3>Information</h3>
<p>There are 8 Input files.</p>
<ul>
<li>Input #1: $1 \le n \le 50000$, TL=1s</li>
<li>Input #2: $1 \le T \le 1000, \ 1 \le n \le 5 \times 10^7$, TL=5s</li>
<li>Input #3: $1 \le T \le 300, \ 1 \le n \le 5 \times 10^8$, TL=5s</li>
<li>Input #4: $1 \le T \le 80, \ 1 \le n \le 5 \times 10^9$, TL=5s</li>
<li>Input #5: $1 \le T \le 30, \ 1 \le n \le 5 \times 10^{10}$, TL=10s</li>
<li>Input #6: $1 \le T \le 10, \ 1 \le n \le 5 \times 10^{11}$, TL=10s</li>
<li>Input #7: $1 \le T \le 3, \ 1 \le n \le 5 \times 10^{12}$, TL=10s</li>
<li>Input #8: $T=1, \ 1 \le n \le 5 \times 10^{13}$, TL=10s</li>
</ul>
<p>My unoptimized C++ solution runs in 8.9 sec (total time). And with some constant optimization, now my C++ solution runs in 1.03 sec (total time).</p>