<p>Disputes between two warring parties over possession of properties are often settled amicably with the intervention of a third party. You are required to write a program on behalf of a consultancy firm that settles disputes amicably over possession of properties between two warring parties.</p>
<p>
The dispute between two warring parties A and B, is over a set of n profit making industrial units (PMIU) that currently make profits P1, P2,..., Pn . Assume that n is an even number less than 20. Each profit is a distinct integer representing rounded profit in crores of rupees. A profit identifies a PMIU and determines its valuation. For a subset of PMIU, the product of all profits from PMIU in the subset determines the total valuation of the subset. The two warring parties have agreed to accept a solution that divides the set of n PMIU into two disjoint subsets satisfying the following conditions:
</p>
<ol>
<li>The total number of PMIU in each subset is n/2 .</li>
<li>The total valuation of each subset is the same.</li>
<li>The subset with higher total sum of profits is allocated to A.</li>
</ol>
<p>
Write a program that determines the subset of PMIU to be allocated to A, assuming that there exists a unique solution to the problem.
</p>
<p>
As a simple example consider 6 PMIU with profits 2, 4, 5, 12, 15 and 18. The subset of PMIU allocated to A is {2, 12, 15}.
</p>
<h3>Input</h3>
<p>The input may contain multiple test cases.</p>
<p>For each test case there is a single input line. The line gives a set of distinct integers representing profits of PMIU.</p>
<p>The input terminates with a line containing 0 as input.
</p>
<h3>Output</h3>
<p>
For each test case there is only one output line. The line prints the subset of PMIU allocated to A in ascending order of profits.
</p>

<h3>Example</h3>
<pre><b>Sample Input</b>
8 12 10 15
2 4 5 12 15 18
0

<b>Sample Output</b>
8 15
2 12 15
</pre>