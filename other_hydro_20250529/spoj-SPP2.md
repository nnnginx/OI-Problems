<p><em> </em></p>
<p><em>Sequence <em>(a<sub>i</sub>)</em> of natural numbers is defined as follows:<br><br><em>a<sub>i</sub> = b<sub>i</sub></em> (for <em>i &lt;= m</em>)<br><em>a<sub>i</sub> = c<sub>1</sub>a<sub>i-1</sub> + c<sub>2</sub>a<sub>i-2</sub> + ... + c<sub>t</sub>a<sub>i-t</sub></em> (for <em>i &gt; t</em>)<br><br>where <em>b<sub>j</sub></em> and <em>c<sub>j</sub></em> are given natural numbers. Your task is to compute <em>a<sub>n</sub></em> and output it modulo 10<sup>9</sup>+7.</em></p>
<p><em> </em></p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>The above is the description of the original problem <a href="http://spoj.com/problems/SEQ">SEQ</a>. However, to be a problem in a regional contest, the description will be slightly modified to make the problem a little bit complicated: for almost all integers <em>i</em> &gt; <em>m</em>, a<sub>i</sub> follows the formula given above, but there are <strong>q</strong> exceptions n<sub>1</sub>, n<sub>2</sub>, ..., n<sub>q</sub>:</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<div><em>a<sub>n<sub>i</sub></sub> = d<sub>i1</sub>a<sub>n<sub>i</sub>-1</sub> + d<sub>i2</sub>a<sub>n<sub>i</sub>-2</sub> + ... + d<sub>it<sub>i</sub></sub>a<sub>n<sub>i</sub>-t<sub>i</sub></sub> (for 1 &lt;= <em>i</em> &lt;= <strong>q</strong>)</em></div>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>For each test case, the first line contains three integers <strong>n</strong> (<strong>m</strong> &lt; <strong>n</strong> &lt;= 10<sup>9</sup>), <strong>m</strong> (1 &lt;= <strong>m</strong> &lt;= 100), <strong>q</strong> (0 &lt;= <strong>q</strong> &lt;= 100). The second line contains <strong>m</strong> integers b<sub>1</sub>, b<sub>2</sub>, ..., b<sub>m</sub>. The following line contains several integers, first comes t (t ¡Ü 100), then t integers c<sub>1</sub>, c<sub>2</sub>, ..., c<sub>t</sub>. The following <strong>q</strong> lines describe <strong>q</strong> special cases of the recurrent formula, each containing several integers, namely n<sub>i</sub>, t<sub>i</sub> (t<sub>i</sub> ¡Ü 100, t<sub>i</sub> &lt; n<sub>i</sub>), d<sub>i1</sub>, d<sub>i2</sub>, ..., d<sub>it<sub>i</sub></sub>, as mentioned earlier. It is satisfied that all n<sub>i</sub> are distinct. All integers are non-negative. Unless specified, all integers are not greater than 10<sup>9</sup>. Input is terminated by EOF. You might assume that all given data is correct. That is to say, all the required numbers can be fixed uniquely by the given input data.</p>
<h3>Output</h3>
<p>For each test case output the answer in a single line. Refer to the example for more format details.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
7 5 0
1 1 2 3 5
2 1 1
10 5 1
1 1 2 3 5
2 1 1
10 2 1 2

<strong>Output:</strong>
Case 1: 13
Case 2: 76
</pre>
<p>&nbsp;</p>
<p>&nbsp;</p>