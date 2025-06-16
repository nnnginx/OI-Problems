<p>Solar cycle predictions are used by various agencies and many industry groups.
 The solar cycle is important for determining the lifetime of satellites in low-Earth orbit,
 as the drag on the satellites correlates with the solar cycle [...].
 <a href="http://www.swpc.noaa.gov/products/solar-cycle-progression">(NOAA)</a>
 </p>


<div align="center"><img style="width: 50%; height: 50%" title="400 Years of Sunspot Observation" src="../../content/francky:Sun400" alt="400 Years of Sunspot Observation">
<a href="http://en.wikipedia.org/wiki/Solar_cycle">(Solar Cycle)</a>
</div>

<p> <br></p>

<div align="center">
	<img style="width: 20%; height: 20%" title="Pred-2008" src="../../content/francky:Sun2008" alt="">
	<img style="width: 20%; height: 20%" title="Pred-2012" src="../../content/francky:Sun2012" alt="">
	<img style="width: 20%; height: 20%" title="Pred-2014" src="../../content/francky:Sun2014" alt="">
	<img style="width: 20%; height: 20%" title="Pred-2016" src="../../content/francky:Sun2016" alt="">
</div>
<p>Sunspot Number Progression : Observed data through May 2008 ; Dec 2012 ; Nov 2014 ; Jun 2016</p>

<p> <br> <br> </p>
<p>The goal of the problem is to propose a perfect prediction center, with not so weak constraints.</p>

<p>Let us consider periodic functions from <strong>Z</strong> to <strong>R</strong>.</p>

<pre>	<span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">f</span>(x): <span style="color: #008800; font-weight: bold">return</span> [<span style="color: #0000DD; font-weight: bold">4</span>, <span style="color: #333333">-</span><span style="color: #0000DD; font-weight: bold">6</span>, <span style="color: #0000DD; font-weight: bold">7</span>][x<span style="color: #333333">%</span><span style="color: #0000DD; font-weight: bold">3</span>] <span style="color: #888888"># (with Python notations)</span>
	<span style="color: #888888"># 4, -6, 7, 4, -6, 7, 4, -6, 7, 4, -6, 7, 4, -6, 7, ...</span>
</pre>

<p>
For example, <em>f</em> is a 3-periodic function, with <em>f</em>(0) = <em>f</em>(3) = <em>f</em>(6) = <em>f</em>(9) = 4. <br>
With a simplified notation we will denote f as [4, -6, 7].


<br>
For two periodic functions (with integral period), the quotient of periods will be rational, in that case it can be shown that the sum of the functions is also a periodic function. Thus, the set of all such functions is a vector space over <strong>R</strong>.
</p>

<p>
For that problem, we consider a function that is the sum of several periodic functions all with as period an integer <em>N</em> at maximum. You will be given some starting values, you'll have to find new ones.
</p>

<h3>Input</h3>
<p>
On the first line, you will be given an integer <em>N</em>.<br>
On the second line, you will be given integers <em>y</em> : the first (0-indexed) <em>N×N</em> values of a periodic function <em>f</em>
 that is sum of periodic functions all with as period an integer <em>N</em> at maximum.<br>
On the third line, you will be given <em>N×N</em> integers <em>x</em>.
</p>

<h3>Output</h3>
<p>
	Print <em>f(x)</em> for all required <em>x</em>. See sample for details.
</p>

<h3>Example</h3>

<pre><b>Input:</b>
3
15 3 17 2 16 4 15 3 17
10 100 1000 10000 100000 1000000 10000000 100000000 1000000000

<b>Output:</b>
16 16 16 16 16 16 16 16 16
</pre>

<h3>Explanation</h3>
<p>For example <em>f</em> can be seen as the sum of three periodic functions : [10] + [5, -8] + [0, 1, 2] (with simplified notations ; periods are 1,2 and 3)<br>
In that case <em>f</em>(10) = [10][10%1] + [5, -8][10%2] + [0, 1, 2][10%3] = 10 + 5 + 1 = 16, and so on.
</p>

<h3>Constraints</h3>
<pre>N &lt; 258
abs(y) &lt; 10^9
0 &lt;= x &lt; 10^9
</pre>
For PERIOD4 you can have AC with <em>O</em>(<em>N</em>⁶) method,  for PERIOD3 the awaited solution is about π⁶/27 faster.<br>
For PERIOD5 a new complexity is awaited.
<p></p>

<h3>Informations</h3>
<p>You can safely assume output fit in a signed 32bit container.
There's 6 input files, with increasing value of <em>N</em>.
My modest C code ended in 1.27s ; no optimization.
Some details (#i, <em>N</em>, TL, t) :
(#0, around 50, 1s, 0s),
(#1, around 50, 1s, 0s),
(#2, around 100, 1s, 0.04s),
(#3, around 150, 3s, 0.14s),
(#4, around 200, 7s, 0.36s),
(#5, around 250, 15s, 0.74s).
<br>
You may first try the medium edition <a href="http://www.spoj.com/problems/PERIOD3/">PERIOD3</a>. <strong>Have fun ;-)</strong>
</p>

<p>(Edit 2017-02-11 ; compiler update ; here ×2 speedup) Some updated details (#i, <em>N</em>, TL, t) :
(#0, around 50, 1s, 0s),
(#1, around 50, 1s, 0s),
(#2, around 100, 1s, 0.02s),
(#3, around 150, 3s, 0.07s),
(#4, around 200, 7s, 0.18s),
(#5, around 250, 15s, 0.36s).
</p>