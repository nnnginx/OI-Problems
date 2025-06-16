<p>A 123 sequence is defined as a non-decreasing sequence of length&gt;=2, where each number is 1 or 2 or 3. The difference between all unique pairs of numbers is given i.e. for a 123 sequence a<sub>1</sub>, a<sub>2</sub>, a<sub>3</sub>, ..., an the differences are a<sub>j</sub>-a<sub>i</sub> for 1&lt;=i&lt;j&lt;=n.</p>
<p>Since the 123 seq contains only 1, 2, 3 the difference between any pair can be 0, 1, 2. Given the number of 0s, 1s, 2s in the difference sequence X, Y, Z respectively, your task is to find the number of distinct 123 sequences that could result in X, Y, Z.</p>
<p>Two 123 sequences A and B are considered different if there exists atleast one i such that A<sub>i</sub> is not equal to B<sub>i</sub>.</p>
<h3>Input</h3>
<p>First line of the input contains the number of test cases T. <strong>T&lt;=10000</strong>. Then follow T lines each containing 3 space separated integer X, Y, Z. <strong>0&lt;=X,</strong><strong>Y,</strong><strong>Z,&lt;=10<sup>8</sup></strong>. <strong>X+</strong><strong>Y+</strong><strong>Z&gt;0</strong>.</p>
<h3>Output</h3>
<p>For each test case output the number of distinct 123 sequences in a separate line.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>3<br>0 2 1<br>1 2 3<br>1 3 2<br><br><strong>Output:</strong><br>1<br>0<br>2<br></pre>
<h3>Explanation</h3>
<p>For the third test case the 123 sequences are 1, 2, 3, 3 and 1, 1, 2, 3.</p>