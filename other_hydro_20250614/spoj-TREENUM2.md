<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>A number is called a tree_num while it can be partition into sum of some distinct powers of 3 with natural exponent. Example : 13 and 90 are tree_num because 13 = 3<sup>2</sup> + 3<sup>1</sup> + 3<sup>0</sup>, 90 = 3<sup>4</sup> + 3<sup>2</sup>.</p>
<p>Let $tree\_num(i)$ be the i-th largest tree_num.</p>
<p>Example : $tree\_num(1) = 1$, $tree\_num(2) = 3$, $tree\_num(5) = 10$, ¡­</p>
<p>Let $$F(L, R) = \sum _{i = L}^R tree\_num(i)$$</p>
<p><span style="white-space: pre;"> </span></p>
<p>Your task is to find F(L, R) with some given L, R.</p>
<h3>Input</h3>
<p>- First line : an integer T ¨C number of testcases (1 ¡Ü T ¡Ü 100000)</p>
<p>- Next T lines : each line contains two number ¨C L and R (1 ¡Ü L ¡Ü R ¡Ü 10<sup>18</sup>)</p>
<h3>Output</h3>
<p>-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; For each pair (L, R), output a line containing the value F(L, R). Since those values can be very large, just output them modulo 2<sup>32</sup></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p>5</p><p>1 3</p><p>3 3</p><p>4 5</p><p>6 7</p><p>2 5</p>
<strong>Output:</strong>
<p>8</p><p>4</p><p>19</p><p>25</p><p>26</p></pre>