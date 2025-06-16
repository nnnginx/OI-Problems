<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>Every day, Danny buys one sweet from the candy store and     eats it. The store has $m$     types of sweets, numbered from      $1$ to      $m$. Danny knows that a balanced diet     is important and is applying this concept to his sweet     purchasing. To each sweet type      $i$, he has assigned a <em>target     fraction</em>, which is a real number      $f_ i$ (     $0 &lt; f_ i \le 1$). He wants the     fraction of sweets of type      $i$ among all sweets he has eaten to     be roughly equal to $f_     i$. To be more precise, let      $s_ i$ denote the number of sweets of     type $i$ that Danny has     eaten, and let $n = \sum _{i=1}^     m s_ i$. We say the set of sweets is <em>balanced</em> if for every $i$ we     have</p>
<p>\[ n f_ i - 1 &lt; s_ i     &lt; n f_ i + 1. \]</p>
<p>Danny has been buying and eating sweets for a while and     during this entire time the set of sweets has been balanced. He     is now wondering how many more sweets he can buy while still     fulfilling this condition. Given the target fractions     $f_ i$ and the sequence of     sweets he has eaten so far, determine how many more sweets he     can buy and eat so that at any time the set of sweets is     balanced.</p>
<h3>Input</h3>
<p>The input consists of multiple test cases. Please process until EOF is reached.</p>
<p>Each test case consists of three lines. The first line contains     two integers $m$     ($1 \le m \le 10^5$),     which is the number of types of sweets, and      $k$ ($0     \le k \le 10^5$), which is the number of sweets Danny     has already eaten.</p>
<p>The second line contains      $m$ positive integers      $a_1, \ldots , a_ m$. These numbers     are proportional to $f_1, \ldots     , f_ m$, that is,      $\displaystyle f_ i = \frac{a_ i}{\sum _{j =     1}^ m a_ j}$. It is guaranteed that the sum of all     $a_ j$ is no larger than     $10^5$.</p>
<p>The third line contains      $k$ integers      $b_1, \ldots , b_ k$ (     $1 \le b_ i \le m$), where each     $b_ i$ denotes the type of     sweet Danny bought and ate on the      $i^\text {th}$ day. It is guaranteed     that every prefix of this sequence (including the whole     sequence) is balanced.</p>
<h3>Output</h3>
<p>For each test case, display the maximum number of additional sweets that Danny     can buy and eat while keeping his diet continuously balanced.     If there is no upper limit on the number of sweets, display the     word <em>forever</em>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
6 5
2 1 6 3 5 3
1 2 5 3 5
6 4
2 1 6 3 5 3
1 2 5 3

<strong>Output:</strong>
1
forever
    </pre>