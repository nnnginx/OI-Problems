<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>A large part of the world economy depends on oil, which is     why research into new methods for finding and extracting oil is     still active. Profits of oil companies depend in part on how     efficiently they can drill for oil. The International Crude     Petroleum Consortium (ICPC) hopes that extensive computer     simulations will make it easier to determine how to drill oil     wells in the best possible way.</p>
<p>Drilling oil wells optimally is getting harder each day ¨C     the newly discovered oil deposits often do not form a single     body, but are split into many parts. The ICPC is currently     concerned with stratified deposits, as illustrated below.</p>
<p><img style="width: 800px; height: 420px;" src="../../../content/john_jones:fn16oil.png" alt=""></p>
<p>To simplify its analysis, the ICPC considers only the     2-dimensional case, where oil deposits are modeled as     horizontal line segments parallel to the earth¡¯s surface. The     ICPC wants to know how to place a single oil well to extract     the maximum amount of oil. The oil well is drilled from the     surface along a straight line and can extract oil from all     deposits that it intersects on its way down, even if the     intersection is at an endpoint of a deposit. One such well is     shown as a dashed line in Figure, hitting three     deposits. In this simple model the amount of oil contained in a     deposit is equal to the width of the deposit. Can you help the     ICPC determine the maximum amount of oil that can be extracted     by a single well?</p>
<h3>Input</h3>
<p>Multiple test cases. Please process until EOF is reached. For each test case:</p>
<p>The first line of input contains a single integer     $n$ (     $1 \leq n \leq 2\, 000$), which is the     number of oil deposits. This is followed by      $n$ lines, each describing a single     deposit. These lines contain three integers      $x_0$,      $x_1$, and      $y$ giving the deposit¡¯s position as     the line segment with endpoints      $(x_0,y)$ and      $(x_1,y)$. These numbers satisfy     $|x_0|, |x_1| \leq 10^6$     and $1 \le y \le 10^6$. No     two deposits will intersect, not even at a point.</p>
<h3>Output</h3>
<p>For each test case, display the maximum amount of oil that can be extracted by a     single oil well.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5
100 180 20
30 60 30
70 110 40
10 40 50
0 80 70
3
50 60 10
-42 -42 20
25 0 10

<strong>Output:</strong>
200
25

</pre>