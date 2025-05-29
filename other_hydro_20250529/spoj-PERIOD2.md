<p>Milankovitch's cycle theory  is an example with cumulative effect of several periodic functions.<br>
We can study past climatic patterns on Earth through orbital forcing.
</p>

<div align="center"><img style="width: 50%; height: 50%" title="http://en.wikipedia.org/wiki/Milankovitch_cycles" src="../../content/francky:Milankovitch" alt="Milankovitch cycles - image">
</div>

<p>Let us consider periodic functions from <strong>Z</strong> to <strong>R</strong>.</p>

<pre>	<span style="color: #008800; font-weight: bold">def</span> <span style="color: #0066BB; font-weight: bold">f</span>(x): <span style="color: #008800; font-weight: bold">return</span> [<span style="color: #0000DD; font-weight: bold">4</span>, <span style="color: #0000DD; font-weight: bold">-6</span>, <span style="color: #0000DD; font-weight: bold">7</span>][x<span style="color: #333333">%</span><span style="color: #0000DD; font-weight: bold">3</span>] <span style="color: #888888"># (with Python notations)</span>
	<span style="color: #888888"># 4, -6, 7, 4, -6, 7, 4, -6, 7, 4, -6, 7, 4, -6, 7, ...</span>
</pre>

<p>
For example, <em>f</em> is a 3-periodic function, with <em>f</em>(0) = <em>f</em>(3) = <em>f</em>(6) = <em>f</em>(9) = 4. <br>
With a simplified notation we will denote f as [4, -6, 7]. 

<br>
For two periodic functions (with integral period), the quotient of periods will be rational,
in that case it can be shown that the sum of the functions is also a periodic function.<br>
Thus, the set of all such functions is a vector space over <strong>R</strong>.
</p>

<p>
Our interest, in this problem, will be the smallest common period of sums of periodic functions whose period is an integer, bounded by some <em>N</em>.
</p>




<h3>Input</h3>
<p>The first line contains an integer <em>T</em>, the number of test cases.<br>
On the next <em>T</em> lines, you will be given two integers <em>N</em> and <em>M</em>.<br>
Consider the family of any finite sum of ( <em>n</em>-periodic functions with <em>n</em> in [1..<em>N</em>] ).<br>
All those functions share a common smallest period.
</p>

<h3>Output</h3>
<p>
	Print the smallest common period of that family.
	As the answer can get very big, simply output it modulo <em>M</em>.
</p>

<h3>Example</h3>

<pre><b>Input:</b>
3
2 10
3 100
4 7

<b>Output:</b>
2
6
5
</pre>

<h3>Explanation</h3>
<p>
The first case is trivial.<br>
For the second case, for example if <em>f</em> = [0] + [5, ¦Ð] + [0, -e , 1] then <em>f</em> can be written as [5, ¦Ð-e, 6, ¦Ð, 5-e, ¦Ð+1] and is 6-periodic ; 6 is smallest common period for any sum of <em>n</em>-periodic function when <em>n</em> is bounded by 3.<br>
For the third case, 12%7 is equal to 5.
</p>

<h3>Constraints</h3>
<pre>0 &lt; T &lt; 10^3
0 &lt; N &lt; 10^7
1 &lt; M &lt; 10^9
</pre>
<p>Uniform random input, one input file.</p>

<h3>Information</h3>
<p>Constraints allow my optimized Python code to get AC in 12s, and a poor C code in 4s.
The curious fact is that on my hardware the corresponding times are quite the same, and I've set the constraints with that in mind... curious for me.</p>
<p>Edit 2017-02-11 : with compiler changes, now the two times are similar 3.5s (poor.c) ; 3.57s (good.py). The new TL is set at 7s. It allows JAVA too.
</p>