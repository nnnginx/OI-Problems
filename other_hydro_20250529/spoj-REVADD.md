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
<p>
A number $N$ is called <b>special</b> iff it can be written as
$$
  N = \mathrm{reverse}(N_1) + N_1 = \mathrm{reverse}(N_2) + N_2,
$$
where $N_1$ and $N_2$ are some positive integers and their number of digits (lengths) are different.
</p>
<p>
For example, $121$ is a special number since
$$
\begin{aligned}
  121 &amp;= \mathrm{reverse}(74) + 74 = \mathrm{reverse}(110) + 110 \\
      &amp;= 47 + 74 = 11 + 110.
\end{aligned}
$$
</p>
<p>There are only two special number less than $10,000$.</p>
<p>Find the first 5,000 smallest special numbers.</p>

<h3>Input</h3>
<p>This problem has no input data.</p>
<h3>Output</h3>
<p>Output the first 5,000 special numbers in ascending order. (One special number per one line.)</p>

<h3>Example</h3>
<h4>Output:</h4>
<pre>121
1111
...
[4998 lines]
...
</pre>
<h3>Information</h3>
<p>Source Limit is 10 KB.</p>