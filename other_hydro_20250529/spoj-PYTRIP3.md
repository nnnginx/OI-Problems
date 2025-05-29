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
<p>We define a Pythagorean triple as a set of three positive integers $a$, $b$ and $c$ which satisfy $a^2 + b^2 = c^2$.</p>
<p>Let $P(N)$ denote the number of Pythagorean triples whose hypotenuses ($= c$) are less than or equal to $N$ (i.e. $c \le N$).</p>
<p>Given $N$, find $P(N)$.</p>
<h3>Input</h3>
<p>The first line of input contains a positive integer $N$.</p>
<h3>Output</h3>
<p>Print on a single line the value of $P(N)$.</p>
<h3>Constraints</h3>
<p>$1 \le N \le 1234567891011$</p>
<h3>Example</h3>
<pre><strong>Input1:</strong>
5

<strong>Output1:</strong>
1

<strong>Input2:</strong>
15

<strong>Output2:</strong>
4

<strong>Input3:</strong>
10000

<strong>Output3:</strong>
12471

<strong>Input4:</strong>
1000000000000

<strong>Output4:</strong>
4179478903392</pre>
<h3>Explanation for Input2</h3>
<p>There are four Pythagorean triples: $\{3, 4, 5\}$, $\{5, 12, 13\}$, $\{6, 8, 10\}$, $\{9, 12, 15\}$</p>
<h3>Information</h3>
<p>There are 15 test cases.</p>
<p>The sum of the time limits is 93 sec. (My solution runs in 5.4 sec.)</p>
<p><strong>Source Limit is 5 KB.</strong></p>