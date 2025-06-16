<p>A fraction tree is an infinite binary tree defined as follows:</p>
<p>1) Every node of tree contains a fraction</p>
<p>2) Root of tree contains the fraction 1/1</p>
<p>3) Any node with fraction i/j has two children : left child with fraction i/(i+j) and right child with fraction (i+j)/j</p>
<p>For example , fraction tree upto 3 levels is as shown:</p>
<h3 style="text-align: center;"><img title="Fraction tree upto 3 levels" src="../../content/francky:CW" alt="Fraction tree upto 3 levels" width="428" height="219"></h3>

<p>We number the nodes according to increasing levels ( root is at level 1) and at any same level , nodes are numbered from left to right. So first node holds the fraction 1/1 , second one holds 1/2 , third one holds 2/1 fourth one holds 1/3 and so on.</p>
<p>Your task is simple. Given a number n , you are to find the fraction at the nth node.</p>

<h3>Input</h3>
<p>Every line of the input contains a single number n. You are to find the fraction at nth node of fraction tree. Input file terminates with a 0 which is not to be processed.</p>

<h3>Output</h3>
<p>For each input , print numerator and denominator of the lowest form of the fraction seperated by a /. Output of each case to be done in seperate lines.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
1
2
3
7
0

<strong>Output:</strong>
1/1
1/2
2/1
3/1</pre>

<h3>Constraints</h3>
<p>1 &lt;= # of test cases &lt;= 30000, 1 &lt;= N &lt;= 10^10</p>