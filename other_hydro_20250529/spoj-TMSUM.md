<p>You are given a set S of n elements. Do you know how many subsets the set has? It is 2^n where n is the number of elements in S.</p>
<p>For example, consider a set S of 3 elements. S= {1, 2, 3} so S has 2^3=8 subsets. They are {1}, {2}, {3}, {1,2}, {2,3}, {1,3}, {1,2,3}, {}. Here {} is empty set.</p>
<p>In the above example number of subsets of S having at most 2 elements excluding empty set are {1}, {2}, {3}, {1,2}, {2,3}, {1,3}.</p>
<p>Find subsets which have at most 2 elements excluding empty set in which each element of S must belong to a single a subset i.e. if we take subset for example {1} then we can¡¯t take other subsets containing element 1. Now sum the product of the subsets containing 2 elements with the value of subsets containing single element. Your target will be maximizing this sum.</p>
<p>For example consider a set S= {1, 2, 3, 4, 5, 6}. So the subsets of S having at most 2 elements excluding empty set are {1}, {2}, {3}, {4}, {5}, {6}, {1,2}, {1,3}, {1,4}, {1,5}, {1,6}, {2,3}, {2,4}, {2,5}, {2,6}, {3,4}, {3,5}, {3,6}, {4,5}, {4,6}, {5,6}.</p>
<p>Now we can take subsets of {5,6}, {4,3} and {1,2} which contains all 6 elements of S then total sum&nbsp; will be = (5*6)+(4*3)+(1*2) = 44. On the other hand if we take subsets of {5, 6}, {4, 3} and {1} &amp; {2} then total sum will be= (5*6) + (4*3) +1+2=45 which is greater than the previous one.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line of the input will be an integer T to represent the number of test cases. For each case there will be two lines. The first line contains integer&nbsp;<em>n</em>&nbsp;¡ª the number of distinct elements in the given set S. The second line contains&nbsp;<em>n</em>&nbsp;integers&nbsp;s<sub>i</sub>&nbsp;(i=1,2,¡­.., n) ¡ª the elements of the S.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>In a single line, output the maximum sum.</p>
<p>&nbsp;</p>
<p><strong><span style="text-decoration: underline;">Constraints</span></strong></p>
<ul>
<li>1 &lt;= T &lt;= 100</li>
<li>1 &lt;= n &lt;= 100</li>
<li>-10000 &lt;= s<sub>i </sub>&lt;= 10000</li>
</ul>
<p align="left">&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
6
1 2 3 4 5 6
3
1 2 3<br>&nbsp;</pre>
<pre><strong>Output:</strong>
45
7
</pre>