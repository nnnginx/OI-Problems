<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">\smallskip</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The Team is interested in a network of N (2 &lt;= N &lt;= 10^6) cities (conveniently numbered $1..N$), interconnected by M ($1 &lt;= M &lt;= 10^6) one-way flights (similarly numbered $1..M$). Their hometown is city $S$ ($1 &lt;= S &lt;= N$), and the contest will take place in city $E$ ($1 &lt;= E &lt;= N$, $S \neq E$). Flight $i$ goes from city $a_i$ ($1 &lt;= a_i &lt;= N$) to city $b_i$ ($1 &lt;= b_i &lt;= N$, $a_i \neq b_i$), and no two flights connect the same pair of cities in the same direction. In general, no cities are guaranteed to be reachable from other cities by a sequence of flights. However, The Team of course knows that city $E$ is reachable from city $S$ - they're not about to break their streak of triumphant wins!</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">\smallskip</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Now, each city $i$ has a fun value, $f_i$ ($0 &lt;= f_i &lt;= 10^6), associated with it. Along their trip, The Team will take time to have fun at every city they visit, including the first and last. However, though they can visit a city multiple times (including cities $S$ and $E$), or even take a certain flight multiple times, surely this gets boring quickly - therefore, any city's fun can only be had up to once.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">\smallskip</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The Team wants to determine the maximal amount of fun they can have on any sequence of flights that starts at city $S$ and ends at city $E$. Naturally, every member on The Team is so intelligent that they've calculated this value in their heads (and are quite excited about it) - but can you?</div>
<p>It's that time of year again - the best ACM-ICPC team of all time is off to the World Finals! Being the best, they realize that a good performance starts before the contest itself - in order to get into the perfect mindset, they must have as much fun on the trip to the contest site as possible!</p>
<p>The Team is interested in a network of N (2 &lt;= N &lt;= 10^6) cities (conveniently numbered 1..N), interconnected by M (1 &lt;= M &lt;= 10^6) one-way flights (similarly numbered 1..M). Their hometown is city S (1 &lt;= S &lt;= N), and the contest will take place in city E (1 &lt;= E &lt;= N, S != E). Flight i goes from city ai (1 &lt;= ai &lt;= N) to city bi (1 &lt;= bi &lt;= N, ai != bi), and no two flights connect the same pair of cities in the same direction. In general, no cities are guaranteed to be reachable from other cities by a sequence of flights. However, The Team of course knows that city E is reachable from city S - they're not about to break their streak of triumphant wins!</p>
<p>Now, each city i has a fun value, fi (0 &lt;= fi &lt;= 10^6), associated with it. Along their trip, The Team will take time to have fun at every city they visit, including the first and last. However, though they can visit a city multiple times (including cities S and E), or even take a certain flight multiple times, surely this gets boring quickly - therefore, any city's fun can only be had up to once.</p>
<p>The Team wants to determine the maximal amount of fun they can have on any sequence of flights that starts at city S and ends at city E. Naturally, every member on The Team is so intelligent that they've calculated this value in their heads (and are quite excited about it) - but can you?</p>
<h3>Input</h3>
<p>First line: 4 integers, N, M, S, and E</p>
<p>Next N lines: 1 integer, fi, for i = 1..N</p>
<p>Next M lines: 2 integers, ai and bi, for i = 1..M</p>
<h3>Output</h3>
<p>1 integer, the maximal amount of fun The Team can have on their trip.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">5 6 1 4
5
4
5
10
2
1 2
1 3
2 4
3 4
4 5
5 4</span>

<strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">22</span><span style="white-space: normal;"> </span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>The network of cities and flights looks like this (the fun values of cities are shown below them):</p>
<p><img src="../../content/sourspinach:gooda.jpg" alt=""></p>
<p>The optimal route that The Team can take goes through cities 1 -&gt; 3 -&gt; 4 -&gt; 5 -&gt; 4, yielding a total fun value of 5+5+10+2+0=22.</p>
<p> </p>