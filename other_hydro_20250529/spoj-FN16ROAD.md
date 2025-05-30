<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>Ubol Narongdid is the founder of a brash new startup company     called Special D-Liver-E. She wants to corner the market on     overnight deliveries of organs between hospitals in the Phuket     area. For scheduling purposes it is important to have accurate     estimates for the times to perform such deliveries. Several     trips between various hospitals have already been performed, so     delivery times between those pairs of hospitals are known. The     company currently has software to estimate times for other (as     yet untraveled) trips, but so far all the estimates have been     woefully inaccurate.</p>
<p>You have been asked to come up with a method to improve     these estimates. You have at your disposal the following     information: 1) the length (in kilometers) of the roads     connecting each pair of cities in the Phuket area, and 2) a set     of times (in minutes) for various previously executed     deliveries.</p>
<p>You know that roads are one-way, and each road has a fixed     speed limit that lies between      $30$ and      $60$ kilometers per hour. Speed limits     are real-valued and need not be integers. You also know that     delivery trucks always take the route that minimizes distance     traveled, and on each road will always travel at a constant     speed equal to that road��s speed limit. Thus you know, for     example, that if a given trip is      $50$ kilometers, the time it will take     is between $50$ and     $100$ minutes inclusive,     in the absence of any other information. Ah, but you     <em>do</em> have other information, namely the times of     previous deliveries. It is up to you to use it to produce the     best possible estimates.</p>
<h3>Input</h3>
<p>Multiple test cases. Please process until EOF is reached. For each test case:</p>
<p>The input starts with a line containing an integer     $n$ (     $1 \le n \leq 30$) indicating the     number of cities, numbered      $0$ to      $n-1$. After that are      $n$ lines each containing      $n$ integers specifying the distance     in kilometers between cities: the      $j^{\text {th}}$ value on the     $i^{\text {th}}$ line     indicates the distance when traveling directly from city     $i$ to city      $j$. A value of      $-1$ indicates there is no road     directly connecting the two cities, and the distance from any     city to itself is always      $0$; all other distances are positive     and at most $1\, 000$.     There are at most $100$     roads.</p>
<p>Following this is a line with a single integer      $r$ ($1     \le r \leq 100$) indicating the number of previously     executed routes. The next      $r$ lines each contain three integers     $s$,      $d$, and      $t$, where      $s$ and      $d$ are the source and destination     cities and $t$ is how long     the delivery from $s$ to     $d$ took, in minutes.</p>
<p>Finally there is a line containing a single integer     $q$ (     $1 \le q \leq 100$) indicating the     number of future delivery queries. The next      $q$ lines each contain two integers     $s$ and      $d$ giving the source and destination     cities for the query.</p>
<p>You may assume that for each of the      $r+q$ source/destination pairs in the     input there is a unique minimum-distance route.</p>
<h3>Output</h3>
<p>For each test case, display a single line for each query containing the source     and destination cities for that query, followed by the best low     and high bounds on the estimate for the travel time.</p>
<p><strong>The judge is "ignore FP Rounding up to $10^{-2}$".</strong></p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
0 50 -1
55 0 40
-1 40 0
1
0 2 120
3
0 1
1 2
1 0

<strong>Output:</strong>
0 1 50.0 80.0
1 2 40.0 70.0
1 0 55.0 110.0
</pre>