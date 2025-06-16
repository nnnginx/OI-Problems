<p>Given an array of N integers A<sub>1</sub>, A<sub>2</sub>, A<sub>3</sub>…A<sub>N</sub>. If you randomly choose two indexes i ,j such that 1 ≤ i &lt; j ≤ N, what is the expected value of A<sub>i</sub> | A<sub>j</sub>?</p>
<h3>Input</h3>
<p>First line contains an integer T, the number of test cases. Each test case consists of two lines. First line denotes the size of array, N and second line contains N integers forming the array.<br> 1 ≤ T ≤ 10 <br> 2 ≤ N ≤ 100,000 <br> 0 ≤ Ai &lt; 2<sup>31</sup></p>
<h3>Output</h3>
<p>For each test case, print the answer as an irreducible fraction. Follow the format of the sample output. <br> The fraction p/q (p and q are integers, and both p ≥ 0 and q &gt; 0 holds) is called irreducible, if there is no such integer d &gt; 1 that divides both p and q separately.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
2
0 0
3
1 2 3

<strong>Output:</strong>
0/1
3/1
</pre>