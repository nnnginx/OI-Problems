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
<p>Hofstadter¨CConway $10,000 sequence is a famous sequence, which is defined as  $$   a_1 = a_2 = 1,\,   a_{n} = a_{a_{n-1}} + a_{n-a_{n-1}}\, (n \ge 3).  $$</p>
<p>Your task is to find a summatory function $S(n) := \sum\limits_{i=1}^n a_i$ and  compute $S(n)$ <strong>modulo</strong> $10^9$.</p>
<h3>Input</h3>
<p>The first line contains $T$ ($1 \le T \le 10000$), the number of test cases.</p>
<p>Each of the next $T$ lines contains a positive integer $n$ ($1 \le n \le 10^{18}$).</p>
<h3>Output</h3>
<p>For each test case, print $S(n)$ <strong>modulo</strong> $10^9$.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
10
1
2
3
4
5
10
100
1000
1000000
1000000000

<strong>Output:</strong>
1
2
4
6
9
32
2818
269446
334706485
137951847
</pre>
<h3>Explanation</h3>
<p>You can verify that $a_1 = a_2 = 1$, $a_3 = a_4 = 2$ and $a_5 = 3$. So, $S(5) = 9$.</p>
<p>$S(10^9) = 259987670137951847 \equiv 137951847 \pmod{10^9}$.</p>
<h3>Information</h3>
<p>There are 5 input files:</p>
<p>- #1: $n \le 10^{4}$, TL = 2s.</p>
<p>- #2: $n \le 10^{6}$, TL = 2s.</p>
<p>- #3: $n \le 10^{8}$, TL = 3s.</p>
<p>- #4: $n \le 10^{12}$, TL = 5s.</p>
<p>- #5: $n \le 10^{18}$, TL = 12s.</p>
<p>These time limits allow a (slow) Python2 solution to get accepted.</p>