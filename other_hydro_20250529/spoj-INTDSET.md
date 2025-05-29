<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.7.1/katex.min.css" integrity="sha384-wITovz90syo1dJWVh32uuETPVEtGigN07tkttEqPv+uR2SE/mbQcG7ATL28aI9H0" crossorigin="anonymous">
<script src="https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.7.1/katex.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.7.1/contrib/auto-render.min.js"></script>
<script type="text/javascript">// <![CDATA[
document.addEventListener("DOMContentLoaded", function(){
  renderMathInElement(
    document.body,{
      delimiters: [
        {left: "$$", right: "$$", display: true},
        {left: "$", right: "$", display: false}]})});
// ]]></script>

<p>Chiaki has a set $A$ of $n$ intervals, the $i$-th of them is $[l_i, r_i]$. She would like to know the number of such interval sets $S \subset A$: for every interval $a \in A$ which is not in $S$, there exists at least one interval $b$ in $S$ which has non-empty intersection with $a$. As this number may be very large, Chiaki is only interested in its remainder modulo $(10^9+7)$.</p>
<p>Interval $a$ has intersection with interval $b$ if there exists a real number $x$ that $l_a \le x \le r_a$ and $l_b \le x \le r_b$.</p>
<h3>Input</h3>
<p>There are multiple test cases. The first line of input contains an integer $T$, indicating the number of test cases. For each test case:</p>
<p>The first line contains an integer $n$ ($1 \le n \le 2 \times 10^5$) -- the number of intervals.</p>
<p>Each of the following $n$ lines contains two integers $l_i$ and $r_i$ ($1 \le l_i &lt; r_i \le 10^9$) denoting the $i$-th interval.</p>
<p>It is guaranteed that for every $1 \le i &lt; j \le n$, $l_i \ne l_j$ or $r_i \ne r_j$ and that the sum of $n$ in all test cases does not exceed $2 \times 10^5$.</p>
<h3>Output</h3>
<p>For each test case, output an integer denoting the answer.</p>
<h3>Example</h3>
<h4>Input:</h4>
<pre>2
3
1 2
3 4
5 6
3
1 4
2 4
3 4
</pre>
<h4>Output:</h4>
<pre>1
7
</pre>