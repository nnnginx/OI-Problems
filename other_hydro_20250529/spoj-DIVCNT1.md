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
<p>Let $$S_1(n) = \sum _{i=1}^n \sigma_0(i).$$</p>
<p>Given $N$, find $S_1(N)$.</p>
<h3>Input</h3>
<p>First line contains $T$&nbsp;($1 \le T \le 100000$), the number of test cases.</p>
<p>Each of the next $T$ lines contains a single integer $N$. ($1 \le N &lt; 2^{63}$)</p>
<h3>Output</h3>
<p>For each number $N$, output a single line containing $S_1(N)$.</p>
<h3>Example</h3>
<h4>Input</h4>
<pre>5<br>1<br>2<br>3<br>10<br>100
</pre>
<h4>Output</h4>
<pre>1<br>3<br>5<br>27<br>482</pre>
<h3>Explanation for Input</h3>
<p>- $S_1(3) = \sigma_0(1) + \sigma_0(2) + \sigma_0(3) = 1 + 2 + 2 = 5$</p>
<h3>Information</h3>
<p>There are 6 input files.</p>
<p>- Input #1: $1 \le N \le 100000$, TL = 2s.</p>
<p>- Input #2: $1 \le T \le 120,\ 1 \le N \le 10^{15}$, TL = 15s.</p>
<p>- Input #3: $1 \le T \le 60,\ 1 \le N \le 10^{16}$, TL = 15s.</p>
<p>- Input #4: $1 \le T \le 25,\ 1 \le N \le 10^{17}$, TL = 15s.</p>
<p>- Input #5: $1 \le T \le 10,\ 1 \le N \le 10^{18}$, TL = 15s.</p>
<p>- Input #6: $1 \le T \le 5,\ 1 \le N &lt; 2^{63}$, TL = 15s.</p>
<p>My C++ solution runs in about 1.3 seconds for each input #2 - #6.</p>
<h3>Note</h3>
<ul>
<li>Probably, $O(\sqrt{n})$ solutions will not pass.</li>
<li>Intended solutions have a running time of about $O(n^{1/3} \log n)$.</li>
<li>The answer can be $\ge 2^{64}$.</li>
</ul>