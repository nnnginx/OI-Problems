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
<p>Let $C(N, a, b)$ be the number of integer pairs $(x, y)$ in $1 \le x \le a$, $1 \le y \le b$ such that $xy$ is divisible by $N$.</p>
<p>Given $N$, $a$ and $b$, find $C(N, a, b)$ <b>modulo</b> $10^{9}$.</p>

<h3>Input</h3>
<p>The first line contains $T$, the number of test cases.</p>
<p>In each of the next $T$ lines, you are given three numbers $N$, $a$ and $b$.</p>
<h3>Output</h3>
<p>For each test case, print $C(N, a, b)$ <b>modulo</b> $10^{9}$.</p>
<h3>Constraints</h3>
<p>$1 \le T \le 100$</p>
<p>$1 \le N \le 10^{18}$,  $1 \le a \le 10^{18}$,  $1 \le b \le 10^{18}$.</p>
<p>You can assume that the <b>maximum prime factor</b> of $N$ is less than or equal to $10^{5}$.</p>
<h3>Example</h3>
<h4>Input</h4>
<pre>5
1 1 1
2 2 2
10 10 10
100 100 100
1 10000 100000</pre>

<h4>Output</h4>
<pre>1
3
27
520
0
</pre>