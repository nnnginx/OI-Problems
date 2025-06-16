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

<p>A <b>semiprime</b> is a product of two primes such as $9 = 3\times3$ or $580519 = 41\times14159$.</p>

<p>The first ten semiprimes are $4$, $6$, $9$, $10$, $14$, $15$, $21$, $22$, $25$, and $26$.</p>

<p>A <b>run</b> of semiprimes is a contiguous subsequence of semiprimes.  For example, $15$, $21$, $22$ is a run but $9$, $14$, $15$ is not because it skips over $10$.</p>

<p>An <b>even run</b> of semiprimes is a run that contains only even numbers.  The first even run of length $3$ is $454$, $458$, $466$.</p>

<p>Your task is to find the longest even run of semiprimes between $N$ and $M$, inclusive.</p>

<h3>Input</h3>
<p>The first line contains $T$ ($1 \le T \le 20$), the number of test cases.</p>
<p>Each test case is one line containing the integers $N$ and $M$ ($1 \le N \le M \le 10^{14}$, $M - N \le 10^7$).</p>
<p>The sum of the differences $M - N$ over all test cases is at most $10^7$.</p>

<h3>Output</h3>
<p>Print two lines per test case.  On the first line, print the length of the longest even run of semiprimes.  On the second line, print the numbers in the run.</p>
<p>If there are multiple solutions, print the one with the smallest first number.</p>
<p>It is guaranteed that there is at least one even semiprime between $N$ and $M$.</p>

<h3>Example</h3>

<pre><b>Input:</b>
16
4 4
4 6
4 8
4 14
6 10
58 62
1 100
1 1000
1 10000
1 100000
1 1000000
5000000 10000000
247425787142 247425787222
247425000000 247425787221
466937174866 466937199999
99999999000000 100000000000000

<b>Output:</b>
1
4
2
4 6
2
4 6
2
4 6
1
6
2
58 62
2
4 6
3
454 458 466
3
454 458 466
3
454 458 466
5
111614 111626 111634 111638 111646
5
5161318 5161322 5161334 5161342 5161346
8
247425787142 247425787162 247425787166 247425787174 247425787178 247425787198 247425787214 247425787222
7
247425787142 247425787162 247425787166 247425787174 247425787178 247425787198 247425787214
4
466937176054 466937176058 466937176066 466937176078
4
99999999199498 99999999199502 99999999199522 99999999199558
</pre>

<h3>Note</h3>
<p>This problem was inspired by <a href="http://list.seqfan.eu/pipermail/seqfan/2018-April/018634.html">Zak Seidov's post</a> in the SeqFan mailing list.</p>
<br>