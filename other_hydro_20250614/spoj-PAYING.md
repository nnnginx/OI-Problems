<p align="justify">
There are infinitely many coin denominations in the Byteland. They have values of 2^i for i=0,1,2,... . We will say that set of coins c1,c2,...,ck is perfect when it is possible to pay every amount of money between 0 and c1+...+ck using some of them (so {4,2,2,1} is perfect while {8,1} is not). The question is - is it always possible to change given sum n into a perfect set of coins? Of course it is possible ;). Your task will be more complicated: for a sum n you should find minimal number of coins in its perfect representation.
</p>
<h3>Input</h3>
<p align="justify">
First line of input contains one integer c&lt;=50 - number of test cases. Then c lines follow, each of them consisting of exactly one integer n&lt;=10^1000.
</p>
<h3>Output</h3>
<p align="justify">
For each test case output minimal number of coins.
</p>
<h3>Example</h3>
<pre>Input:
5
507
29
8574
233
149

Output:
14
7
21
11
10
</pre>