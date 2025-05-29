<p>Solar cycle predictions are used by various agencies and many industry groups.
 The solar cycle is important for determining the lifetime of satellites in low-Earth orbit,
 as the drag on the satellites correlates with the solar cycle [...].
 <a href="http://www.swpc.noaa.gov/products/solar-cycle-progression">(NOAA)</a>
 </p>


<div align="center"><img style="width: 50%; height: 50%" title="400 Years of Sunspot Observation" src="../../content/francky:Sun400" alt="400 Years of Sunspot Observation">
<a href="http://en.wikipedia.org/wiki/Solar_cycle">(Solar Cycle)</a>
</div>

<p>Sunspot Number Progression : Observed data through May 2008 ; Dec 2012 ; Nov 2014</p>

<div align="center">
	<img style="width: 20%; height: 20%" title="Pred-2008" src="../../content/francky:Sun2008" alt="">
	<img style="width: 20%; height: 20%" title="Pred-2012" src="../../content/francky:Sun2012" alt="">
	<img style="width: 20%; height: 20%" title="Pred-2014" src="../../content/francky:Sun2014" alt="">
</div>
<p>The goal of the problem is to propose a perfect prediction center, with weak constraints.</p>

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
<p>The first line contains an integer <em>T</em>, the number of test cases, then each case will be given on three lines.<br>
On the first line, you will be given an integer <em>N</em>.<br>
On the second line, you will be given integers <em>y</em> : the first (0-indexed) <em>N��N</em> values of a periodic function <em>f</em>
 that is sum of periodic functions all with as period an integer <em>N</em> at maximum.<br>
On the third line, you will be given <em>N��N</em> integers <em>x</em>.
</p>


<h3>Output</h3>
<p>
	Print <em>f(x)</em> for all required <em>x</em>. See sample for details.
</p>

<h3>Example</h3>

<pre><b>Input:</b>
2
2
5 7 5 7
6 7 8 9
3
15 3 17 2 16 4 15 3 17
10 100 1000 10000 100000 1000000 10000000 100000000 1000000000

<b>Output:</b>
5 7 5 7
16 16 16 16 16 16 16 16 16
</pre>

<h3>Explanation</h3>
<p>Test case 1: for example <em>f</em> can be seen as the sum of two periodic functions : [5] + [0, 2] (with simplified notations)<br>
We know that <em>f</em>(0)=5 and <em>f</em>(1)=7, we can deduce that <em>f</em>(6)=5, and so on...
</p>
<p>Test case 2: for example <em>f</em> can be seen as the sum of three periodic functions : [10] + [5, -8] + [0, 1, 2] (with simplified notations). In that case <em>f</em>(10) = [10][10%1] + [5, -8][10%2] + [0, 1, 2][10%3] = 10 + 5 + 1 = 16, and so on.
</p>


<h3>Constraints</h3>
<pre>0 &lt; T &lt; 1024
1 &lt; N &lt; 14 : uniform distribution
abs(y) &lt; 10^9
0 &lt; x &lt; 10^9
</pre>

<h3>Information</h3>
<p>Constraints allow easy coding with various languages. (Edited 2017-02-11 ; with compiler changes)<br>
There's two input files, a small one and a bigger.<br>
My PY3.4 code ended in 0.02+0.28 = 0.30s. My C code in 0.01s.<br>
If you find the constraints too weak, please consider <a href="http://www.spoj.com/problems/PERIOD3/">PERIOD3</a>. <strong>Have fun ;-)</strong>
</p>