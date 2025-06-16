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
<p>A tuple of three numbers ($a$, $b$, $c$) is called a <em>pairwise coprime triple</em> if $\gcd(a, b) = 1$, $\gcd(b, c) = 1$, and $\gcd(c, a) = 1$.</p>
<p>Let $C(n)$ be the number of pairwise coprime triples which satisfy $1 \le a, b, c \le n$.</p>
<p>For example, $C(3)$= #{(1, 1, 1), (1, 1, 2), (1, 1, 3), (1, 2, 1), (1, 2, 3), (1, 3, 1), (1, 3, 2), (2, 1, 1), (2, 1, 3), (2, 3, 1), (3, 1, 1), (3, 1, 2), (3, 2, 1)} = 13.</p>
<p>Given $N$, find $C(N)$.</p>
<h3>Input</h3>
<p>First line contains $T$&nbsp;($1 \le T \le 500$), the number of test cases.</p>
<p>Each line of the next $T$ lines contains a single integer $N$ ($1 \le N \le 100000$).</p>
<p>It is guaranteed that $\sum N \le 100000$ in each input file.</p>
<h3>Output</h3>
<p>For each number $N$, output a single line containing $C(N)$.</p>
<h3>Example</h3>
<h4>Input</h4>
<pre>5<br>1<br>2<br>3<br>10<br>100
</pre>
<h4>Output</h4>
<pre>1<br>4<br>13<br>280<br>282814</pre>
<h3>Information</h3>
<p>There are 5 input files.</p>
<p>My C++ solution runs in 3.04 sec. (in the worst case)</p>