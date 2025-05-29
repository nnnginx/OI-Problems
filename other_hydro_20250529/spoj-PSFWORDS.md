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

<p>A string is called a square string if it can be obtained by concatenating two copies of the same string (i.e. $s=uu$ for some word $u$). For example, "abab", "aa" are square strings, while "aaa", "abba" are not. A string is called prefix-square free if none of its prefixes is a square.</p>
<p>Chiaki would like to know the number of nonempty prefix-square free strings whose length is less than or equal to $n$. The size of the alphabet Chiaki uses is $m$. As this number may be very large, Chiaki is only interested in its remainder modulo $2^{32}$.</p>
<h3>Input</h3>
<p>There are multiple test cases. The first line of input contains an integer $T$ ($1 \le T \le 100$), indicating the number of test cases. For each test case:</p>
<p>The first line contains two integers $n$ and $m$ ($1 \le n \le 100, 1 \le m \le 10^9$) -- the length of the string and the size of the alphabet.</p>
<h3>Output</h3>
<p>For each test case, output an integer denoting the answer.</p>
<h3>Example</h3>
<h4>Input:</h4>
<pre>2
3 2
4 6
</pre>
<h4>Output:</h4>
<pre>8
1266
</pre>
<h3>Information</h3>
<p>There are $5$ input files:</p>
<p>- Input #1: $1 \le T \le 100, 1 \le n \le 10$.</p>
<p>- Input #2: $1 \le T \le 50, 1 \le n \le 30$.</p>
<p>- Input #3: $1 \le T \le 30, 1 \le n \le 60$.</p>
<p>- Input #4: $1 \le T \le 10, 1 \le n \le 80$.</p>
<p>- Input #5: $1 \le T \le 2, 1 \le n \le 100$.</p>