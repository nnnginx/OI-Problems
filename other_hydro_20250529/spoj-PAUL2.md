<p>In number theory there is a very deep unsolved conjecture of the Hungarian Paul Erdős (1913-1996), that there exist infinitely many primes of the form <em>x</em><sup>2</sup>+1, where <em>x</em> is an integer. However, a weaker form of this conjecture has been proved: there are infinitely many primes of the form <em>x</em><sup>2</sup>+<em>y</em><sup>4</sup>. You don't need to prove this, it is only your task to find the number of (positive) primes not larger than <em>n</em> which are of the form <em>x</em><sup>2</sup>+<em>y</em><sup>4</sup> (where <em>x</em> and <em>y</em> are integers).</p>
<h3>Input</h3>
<p>An integer <em>T</em>, denoting the number of testcases (<em>T</em>≤500000). Each of the <em>T</em> following lines contains a positive integer <em>n</em>, where <em>n</em>≤10<sup>12</sup>.</p>
<h3>Output</h3>
<p>Output the answer for each <em>n</em>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
6
1
2
10
9999999
500000000000
1000000000000</pre>
<pre><strong>Output:</strong>
0
1
2
13175
25874902
42377120
</pre>
<pre>ps. my running time on Cube is 9.83 seconds. There is one input set.</pre>
<pre>For a much easier version of this problem see <a href="../HS08PAUL">http://www.spoj.com/problems/HS08PAUL</a>.</pre>