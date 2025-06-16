<script type="text/x-mathjax-config">
MathJax.Hub.Config({
  tex2jax: {
    inlineMath: [['$','$'], ['\\(','\\)']],
    skipTags: ["script","noscript","style","textarea","code"]
  }
});
</script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>

<p>Find the sum of $x$ smallest distinct numbers of the series $2^i \times 3^j$ ($i, j \ge 0$).</p>

<ul>
  <li>the first number of the series is $1 = 2^0 \times 3^0$</li>
  <li>the second number of the series is $2 = 2^1 \times 3^0$</li>
  <li>the third number of the series is $3 = 2^0 \times 3^1$</li>
  <li>the fourth number of the series is $4 = 2^2 \times 3^0$</li>
  <li>the fifth number of the series is $6 = 2^1 \times 3^1$
</li></ul>
<p>
As the sum can be huge print sum <b>modulo</b> $k$.

</p><h3>Input</h3>
<p>
The input contains 2 numbers $x$ and $k$: $1 \le x \le 10^{14}$, $1 \le k \le 10^8$
</p>

<h3>Output</h3>
<p>
The output contains sum of the first $x$ numbers of the series <b>modulo</b> $k$.

</p><h3>Example</h3>

<pre><b>Input:</b>
1 1000

<b>Output:</b>
1

<b>Input:</b>
2 1000

<b>Output:</b>
3</pre>

<p><b>Explanation:</b> $3 = 2^0 \times 3^0 + 2^1 \times 3^0  \pmod{1000}$.</p>

<pre><b>Input:</b>
4 1000

<b>Output:</b>
10

<b>Input:</b>
6 2

<b>Output:</b>
0

<b>Input:</b>
16 1000

<b>Output:</b>
300</pre>