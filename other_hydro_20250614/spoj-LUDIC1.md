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
<p>Find the number of <a href="https://rosettacode.org/wiki/Ludic_numbers">Ludic numbers</a> less than or equal to $N$.</p>

<h3>Input</h3>
<p>The first line contains $T$ ($1 \le T \le 1000$), the number of test cases.</p>
<p>Each test case contains a single integer $N$ ($1 \le N \le 10^9$).</p>

<h3>Output</h3>
<p>For each test case, output the number of Ludic numbers less than or equal to $N$.</p>

<h3>Example</h3>
<h4>Input</h4>
<pre>10
1
2
3
4
5
10
100
1000
1000000
1000000000</pre>

<h4>Output</h4>
<pre>1
2
3
3
4
5
24
142
66164
43956562</pre>

<h3>Note</h3>
<ul>
  <li>See <a href="http://www.spoj.com/problems/LUDIC2/">LUDIC2</a> for a harder version.</li>
  <li>Other references for the Ludic numbers: <a href="http://oeis.org/wiki/Ludic_numbers">Ludic numbers</a> or <a href="http://oeis.org/A003309">A003309</a>.
</li></ul>