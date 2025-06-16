<p>
An <i>n</i>-element permutation is an <i>n</i>-element sequence of distinct numbers
from the set <i>{1, 2, ...,n}</i>. For example the sequence 2,1,4,5,3 is a
5-element permutation.
We are interested in the longest increasing subsequences in a permutation. In this exemplary
permutation they are of length 3 and there are exactly 2 such subsequences: 2,4,5 and 1,4,5.
We will call a number belonging to any of the longest increasing
subsequences a <i>supernumber</i>. In the permutation 2,1,4,5,3 the supernumbers are 1,2,4,5 and 3 is not a supernumber.
Your task is to find all supernumbers for a given permutation.
</p>
<h3> Task </h3>
<p>
Write a program which
</p>
<div align="justify">
<ul>
<li> reads a permutation from standard input,
</li>
<li> finds all its supernumbers,
</li>
<li> writes all found numbers to standard output.
</li>
</ul></div>
<h3> Input </h3>
<p>
Ten test cases (given one under another, you have to process all!).
Each test case consists of two lines.
In the first line there is a number <i>n</i> (1&lt;=n&lt;=100000). In the second
line: an <i>n</i>-element permutation - <i>n</i> numbers separated by single spaces.
</p>
<h3> Output </h3>
<p>
For every test case your program should write two lines. In the first line
- the number of supernumbers in the input permutation. In the second line
the supernumbers separated by single spaces in increasing order.
</p>
<h3>Example</h3>
<pre><tt><b>Input:</b>
5
2 1 4 5 3
[and 9 test cases more]
</tt>
<tt><b>Output:</b>
4
1 2 4 5
[and 9 test cases more]
</tt>
</pre>
<b>Warning: large Input/Output data, be careful with certain languages</b>