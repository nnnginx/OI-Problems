<p>Sequence <em>(a<sub>i</sub>)</em> of natural numbers is defined as follows:<br><br> &nbsp;&nbsp; <em>a<sub>i</sub> = b<sub>i</sub></em> (for <em>i &lt;= k</em>)<br> &nbsp;&nbsp; <em>a<sub>i</sub> = c<sub>1</sub>a<sub>i-1</sub> + c<sub>2</sub>a<sub>i-2</sub> + ... +  c<sub>k</sub>a<sub>i-k</sub></em> (for <em>i &gt; k</em>)<br><br> where <em>b<sub>j</sub></em> and <em>c<sub>j</sub></em> are given natural numbers for <em>1&lt;=j&lt;=k</em>. Your task is to compute <em>a<sub>n</sub></em> for given <em>n</em> and output it modulo <em>10<sup>9</sup></em>.</p>
<h3>Input</h3>
<p>On the first row there is the number <em>C</em> of test cases (equal to about 1000).<br> Each test contains four lines:</p>
<p><em>k</em> - number of elements of <em>(c)</em> and <em>(b)</em> (<em>1 &lt;= k &lt;= 10</em>)<br> <em>b<sub>1</sub>,...,b<sub>k</sub></em> - <em>k</em> natural numbers where <em>0 &lt;= b<sub>j</sub> &lt;= 10<sup>9</sup></em> separated by spaces<br><em>c<sub>1</sub>,...,c<sub>k</sub></em> - <em>k</em> natural numbers where <em>0 &lt;= c<sub>j</sub> &lt;= 10<sup>9</sup></em> separated by spaces<br><em>n</em> - natural number (<em>1 &lt;= n &lt;= 10<sup>9</sup></em>)</p>
<h3>Output</h3>
<p>Exactly <em>C</em> lines, one for each test case: <em>a<sub>n</sub></em> modulo <em>10<sup>9</sup></em></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3 
3 
5 8 2 
32 54 6 
2 
3 
1 2 3 
4 5 6 
6 
3 
24 354 6 
56 57 465 
98765432

<strong>Output:</strong>
8 
714 
257599514
</pre>