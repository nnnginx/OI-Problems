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
<p>Find $N!$ <strong>modulo</strong> $P$.</p>
<h3>Input</h3>
<p>The first line contains $T$ ($1 \le T \le 100,000$), the number of test cases.</p>
<p>Each of the next $T$ lines contains two integers $N$ ($0 \le N \le 10^{11}$) and $P$ ($2 \le P \le 10^{11}$), where $P$ is a prime.</p>
<h3>Output</h3>
<p>For each $N$ and $P$, output $N!$ <strong>modulo</strong> $P$.</p>
<h3>Constraints</h3>
<p>For each input file, It is guaranteed that (the sum of $\sqrt{P}) \le 320000$.</p>
<h3>Example</h3>
<h4>Input</h4>
<pre>3
1000 9907
1000000 9999907
10000000000 99999999907
</pre>
<h4>Output</h4>
<pre>4494
3354924
40583077821</pre>
<h3>Note</h3>
<ul>
<li>Probably, $O(P)$ solutions will not pass.</li>
<li>Intended solutions have a complexity of about $O(\sqrt{P} \log{P})$</li> 
<li>My solution runs in 0.5 seconds for each input file.</li>
</ul>