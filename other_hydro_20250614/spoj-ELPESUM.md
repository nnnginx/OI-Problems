<p>Special Thanks: Jane Alam Jan<br> *At moment in University of Texas at San Antonio - USA</p>
<div>
<p>You will be given <strong>n</strong> integers  <strong>A<sub>1</sub>A<sub>2</sub>A<sub>3</sub>...A<sub>n</sub></strong>. Find a permutation of these <strong>n</strong> integers so that summation of the absolute differences between adjacent elements is maximized.</p>
<p>Suppose <strong>n = 4</strong> and the given integers are <strong> 4 2 1 5</strong>. The permutation <strong> 2 5 1 4</strong> yields the maximum summation. 	For this permutation <strong>sum = abs(2-5) + abs(5-1) + abs(1-4) = 3+4+3 = 10</strong>.</p>
<p>Of all the <strong>24</strong> permutations, you won¡¯t get any summation whose value exceeds <strong>10</strong>. We will call this value, <strong>10</strong>, the <em>elegant permuted sum</em>.</p>
</div>
<h3>Input</h3>
<p>The first line of input is an integer <strong>T</strong> (<strong>T </strong> &lt; 100) that represents the number of test cases. Each case consists of a line that starts with <strong>n </strong>(1 &lt; <strong>n</strong> &lt; 51) followed by n non-negative integers separated by a single  space. None of the elements of the given permutation will exceed 1000.</p>
<h3>Output</h3>
<div>
<p>For each case, output the case number followed by the <em>elegant permuted summation</em>.</p>
</div>
<h3>Example</h3>
<pre><strong>Input:</strong>
3<br>4 4 2 1 5<br>4 1 1 1 1<br>2 10 1

<strong>Output:</strong>
Case 1: 10<br>Case 2: 0<br>Case 3: 9
</pre>