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
<p>This problem is a harder version of <a href="../GCDEX">GCDEX</a>.</p>
<p>Let</p>
<p>$$G(n) = \sum _{i=1}^{n} \sum _{j=i+1}^{n} \gcd(i, j).$$</p>
<p>For example, $G(1) = 0$, $G(2) = \gcd(1, 2) = 1$, $G(3) = \gcd(1, 2) + \gcd(1, 3) + \gcd(2, 3) = 3$.</p>
<p>Given $N$, find $G(N)$ <strong>modulo</strong> $2^{64}$.</p>
<h3>Input</h3>
<p>First line of contains $T$&nbsp;($1 \le T \le 10000$), the number of test cases.</p>
<p>Each of the next $T$ lines contains a single integer $N$. ($1 \le N \le 235711131719$)</p>
<h3>Output</h3>
<p>For each number $N$, output a single line containing $G(N)$ <strong>modulo</strong> $2^{64}$.</p>
<h3>Example</h3>
<h4>Input</h4>
<pre>5<br>1<br>4<br>100<br>1000000<br>100000000000</pre>
<h4>Output</h4>
<pre>0<br>7<br>13015<br>4071628673912<br>5482289417216306300</pre>
<h3>Explanation for Input</h3>
<p>- $G(4) = \gcd(1, 2) + \gcd(1, 3) + \gcd(1, 4) + \gcd(2, 3) + \gcd(2, 4) + \gcd(3, 4) = 7$.</p>
<p>- $G(10^{11}) = 75710919967921216138364 \equiv 5482289417216306300 \pmod{2^{64}}$.</p>
<h3>Information</h3>
<p>There are 7 Input files.</p>
<p>- Input #0: $1 \le T \le 10000$, $1 \le N \le 10000$, TL = 1s.</p>
<p>- Input #1: $1 \le T \le 1000$, $1 \le N \le 10^{7}$, TL = 20s.</p>
<p>- Input #2: $1 \le T \le 200$, $1 \le N \le 10^{8}$, TL = 20s.</p>
<p>- Input #3: $1 \le T \le 40$, $1 \le N \le 10^{9}$, TL = 20s.</p>
<p>- Input #4: $1 \le T \le 10$, $1 \le N \le 10^{10}$, TL = 20s.</p>
<p>- Input #5: $1 \le T \le 2$, $1 \le N \le 10^{11}$, TL = 20s.</p>
<p>- Input #6: $T = 1$, $1 \le N \le 235711131719$, TL = 20s.</p>
<p>My solution runs in 10.7 sec. (total time)</p>
<p><strong>Source Limit is 10 KB</strong>.</p>