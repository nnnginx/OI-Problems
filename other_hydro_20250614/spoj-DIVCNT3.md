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
<p>Let $\sigma_0(n)$ be the number of positive divisors of $n$.</p>
<p>For example, $\sigma_0(1) = 1$, $\sigma_0(2) = 2$ and $\sigma_0(6) = 4$.</p>
<p>Let $$S_3(n) = \sum _{i=1}^n \sigma_0(i^3).$$</p>
<p>Given $N$, find $S_3(N)$.</p>
<h3>Input</h3>
<p>First line contains $T$&nbsp;($1 \le T \le 10000$), the number of test cases.</p>
<p>Each of the next $T$ lines contains a single integer $N$. ($1 \le N \le 10^{11}$)</p>
<h3>Output</h3>
<p>For each number $N$, output a single line containing $S_3(N)$.</p>
<h3>Example</h3>
<h4>Input</h4>
<pre>5<br>1<br>2<br>3<br>10<br>100
</pre>
<h4>Output</h4>
<pre>1<br>5<br>9<br>73<br>2302</pre>
<h3>Explanation for Input</h3>
<p>- $S_3(3) = \sigma_0(1^3) + \sigma_0(2^3) + \sigma_0(3^3) = 1 + 4 + 4 = 9$</p>
<h3>Information</h3>
<p>There are 5 Input files.</p>
<p>- Input #1: $1 \le N \le 10000$, TL = 1s.</p>
<p>- Input #2: $1 \le T \le 300,\ 1 \le N \le 10^{8}$, TL = 20s.</p>
<p>- Input #3: $1 \le T \le 75,\ 1 \le N \le 10^{9}$, TL = 20s.</p>
<p>- Input #4: $1 \le T \le 15,\ 1 \le N \le 10^{10}$, TL = 20s.</p>
<p>- Input #5: $1 \le T \le 2,\ 1 \le N \le 10^{11}$, TL = 20s.</p>
<p>My C++ solution runs in 7.1&nbsp;sec. (total time)</p>
<p><strong>Source Limit is 12 KB</strong>.</p>