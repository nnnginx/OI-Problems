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
<p>The first line contains an integer $N$ ($1 \le N \le 10^{11}$).</p>

<h3>Output</h3>
<p>Output the number of Ludic numbers less than or equal to $N$.</p>

<h3>Example</h3>
<h4>Input</h4>
<pre>100000000000</pre>

<h4>Output</h4>
<pre>3603128157</pre>

<h3>Note</h3>
<ul>
  <li>See <a href="http://www.spoj.com/problems/LUDIC1/">LUDIC1</a> for an easier version.</li>
  <li>Other references for the Ludic numbers: <a href="http://oeis.org/wiki/Ludic_numbers">Ludic numbers</a> or <a href="http://oeis.org/A003309">A003309</a>.
</li></ul>