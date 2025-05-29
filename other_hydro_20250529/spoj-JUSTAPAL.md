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

<p>A palindrome is a symmetrical string, that is, a string read identically from left to right as well as from right to left.</p>
<p>Chiaki has a string $s$ and she can perform the following operation at most once:</p>
<ul>
<li>choose two integer $i$ and $j$ ($1 \le i, j \le |s|$).</li>
<li>swap $s_i$ and $s_j$.</li>
</ul>
<p>Chiaki would like to know the longest palindromic substring of string after the operation.</p>
<h3>Input</h3>
<p>There are multiple test cases. The first line of input contains an integer $T$, indicating the number of test cases. For each test case:</p>
<p>The first line contains a non-empty string $s$ ($1 \le |s| \le 10^6$) consisting of lowercase and uppercase letters.</p>
<p>It is guaranteed that the sum of all $|s|$ does not exceed $10^6$.</p>
<h3>Output</h3>
<p>For each test case, output an integer denoting the answer.</p>
<h3>Example</h3>
<h4>Input:</h4>
<pre>10
a
xxxx
ssfs
aaabbacaa
missimxx
ababababgg
dfsfsdgdg
asdsasdswe
chiaki
teretwer
</pre>
<h4>Output:</h4>
<pre>1
4
3
8
6
9
6
9
3
6
</pre>