<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>My birthday is coming up. Alas, I am getting old and would     like to feel young again. Fortunately, I have come up with an     excellent way of feeling younger: if I write my age as a number     in an appropriately chosen base      $b$, then it appears to be smaller.     For instance, suppose my age in base      $10$ is      $32$. Written in base      $16$ it is only      $20$!</p>
<p>However, I cannot choose an arbitrary base when doing this.     If my age written in base      $b$ contains digits other than     $0$ to      $9$, then it will be obvious that I am     cheating, which defeats the purpose. In addition, if my age     written in base $b$ is too     small then it would again be obvious that I am cheating.</p>
<p>Given my age $y$ and a     lower bound $\ell $ on how     small I want my age to appear, find the largest base     $b$ such that      $y$ written in base      $b$ contains only decimal digits, and     is at least $\ell $ when     interpreted as a number in base      $10$.</p>
<h3>Input</h3>
<p>Multiple test cases. Please process until EOF is reached. Each test case  consists of a single line containing two base 10     integers $y$ (     $10 \le y \le 10^{18}$ ¨C yes, I am     <em>very</em> old) and $\ell     $ ($10 \le \ell \le     y$).</p>
<h3>Output</h3>
<p>For each test case, display the largest base      $b$ as described above in a single line.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
32 20
2016 100

<strong>Output:</strong>
16
42
</pre>