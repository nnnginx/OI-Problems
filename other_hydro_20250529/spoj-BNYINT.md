<p>Please click <a href="http://www.spoj.com/content/john_jones:hangzhou2008.pdf">here</a> to download a PDF version of the contest problems. The problem is problem B in the PDF. Remember that you must use stdin/stdout at SPOJ.</p>

<hr>
<script type="text/x-mathjax-config">
MathJax.Hub.Config({
  tex2jax: {
    inlineMath: [['$','$'], ['\\(','\\)']],
    skipTags: ["script","noscript","style","textarea","code"]
  }
});
</script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
<p>
An antique machine with $\binom{N}{3}$ switches capable of processing integers in the range $0 \ldots 2^N - 1$ has just been discovered. Each switch is associated to a distinct integer in $0 \ldots 2^N - 1$ with exactly three ones in its binary representation. By setting switches associated with number $X_0, X_1, \ldots, X_{M-1}$ to on, any integer $Y$ passing through the machine will render a result of $Y \oplus X_0 \oplus X_1 \oplus \ldots \oplus X_{M-1}$ (here ¡°$\oplus$¡± stands for bitwise- XOR).
</p>

<p>
We are interested in the number of configurations capable of transforming integer $S$ into $T$ with exactly $K$ switches set to on. Could you write a program to help us?
</p>


<h3>Input</h3>
<p>
There are multiple test cases in the input file.
</p>

<p>Each test case starts with two integers, $N$ and $K$ ($1 \le N \le 40, 0 \le K \le \min\{20, \binom{N}{3}\}$), followed by two binary integers, $S$ and $T$, each containing exactly $N$ bits.
</p>
<p>
Two successive test cases are separated by a blank line. A case with $N = 0$ and $K = 0$ indicates the end of the input file, and should not be processed by your program.
</p>

<h3>Output</h3>
<p>
For each test case, please print a single integer, the total number of ways to transform the first integer into the second one. Since the answer could be quite large, you are only required to find the result % $10007$.
</p>

<h3>Example</h3>
<pre><b>Sample Input</b>
4 3
1101
1001

3 1
101
010

5 3
11010
10111

0 0

<b>Output for the Sample Input</b>
Case #1: 1
Case #2: 1
Case #3: 6</pre>