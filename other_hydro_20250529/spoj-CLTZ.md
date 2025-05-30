<p>Let N be a positive integer, Consider the following recurrence: f(1) = N and f(K) = (0.5 + 2.5 * (f(K-1) mod 2)) * f(K-1) + (f(K-1) mod 2) if K&gt;1. For a given N you have to compute the smallest L for which f(L)=1 (such an L always exists for N's in the input).</p>
<h3>Input</h3>
<p>Each line contains a positive integer N in decimal notation.  You can be sure that N and all intermediate results are not  bigger than 10^1888. Input terminated by EOF.</p>
<h3>Output</h3>
<p>For each number N in the input print one line with the value of L in decimal notation.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
2
321
1111111111111
111111111111111111111111111111111111111111111111111111111111
<strong>Output:</strong>
1
2
25
261
1296
</pre>