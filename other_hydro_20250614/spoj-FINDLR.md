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
<p>You are given the first $2K$ integers $a_0, a_1, \ldots, a_{2K-1}$ (modulo $M$) of an infinite integer sequence $(a_i)_{i=0}^{\infty}$ that satisfies an integer-coefficient linear recurrence relation of order $K$.</p>
<p>That is, they satisfy $$   a_n = \sum_{i=1}^{K} c_i a_{n-i} $$ for $n \ge K$, where $c_1, \ldots, c_K$ are integer constants.</p>
<p>Find $a_{2K}$ modulo $M$.</p>
<h3>Input</h3>
<p>The first line contains $T$ ($1 \le T \le 4000$), the number of test cases.</p>
<p>Each test case consists of two lines:</p>
<ul>
<li>First line contains $K$ ($1 \le K \le 50$) and $M$ ($1 \le M &lt; 2^{31}$).</li>
<li>Next line contains $2K$ integers $a_0, a_1, \ldots, a_{2K-1}$ (modulo $M$).</li>
</ul>
<p><strong>Note:</strong> $M$ is <strong>not necessarily a prime</strong>.</p>
<h3>Output</h3>
<p>For each test case, output $a_{2K}$ modulo $M$.</p>
<h3>Example</h3>
<h4>Input</h4>
<pre>6
1 16
4 8
1 10
4 8
2 64
13 21 34 55
2 27
13 21 7 1
3 1000000007
32 16 8 4 2 1
2 64
13 21 34 56</pre>
<h4>Output</h4>
<pre>0
6
25
8
500000004
40</pre>