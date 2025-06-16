<p>Sequence <i>(a<sub>i</sub>)</i> of natural numbers is defined as follows:<br><br>

   <i>a<sub>i</sub> = b<sub>i</sub></i> (for <i>i &lt;= k</i>)<br>
   <i>a<sub>i</sub> = c<sub>1</sub>a<sub>i-1</sub> + c<sub>2</sub>a<sub>i-2</sub> + ... + 
c<sub>k</sub>a<sub>i-k</sub></i> (for <i>i &gt; k</i>)<br><br>

where <i>b<sub>j</sub></i> and <i>c<sub>j</sub></i> are given natural numbers for <i>1&lt;=j&lt;=k</i>. Your task is to compute <i>a<sub>m</sub></i> + <i>a<sub>m+1</sub></i> + <i>a<sub>m+2</sub></i> + ... + <i>a<sub>n</sub></i> for given <i>m</i> &lt;= <i>n</i> and output it modulo a given positive integer p.

</p><h3>Input</h3>
<p>On the first row there is the number <i>C</i> of test cases (equal to about 50).<br>
Each test contains four lines:<br>
<i>k</i> - number of elements of <i>(c)</i> and <i>(b)</i> (<i>1 &lt;= k &lt;= 15</i>)<br>

<i>b<sub>1</sub>,...,b<sub>k</sub></i> - <i>k</i> natural numbers where <i>0 &lt;= b<sub>j</sub> &lt;= 10<sup>9</sup></i> separated by spaces<br>

<i>c<sub>1</sub>,...,c<sub>k</sub></i> - <i>k</i> natural numbers where <i>0 &lt;= c<sub>j</sub> &lt;= 10<sup>9</sup></i> separated by spaces<br>

<i>m</i>, <i>n</i>, <i>p</i> - natural numbers separated by spaces (<i>1 &lt;= m &lt;= n &lt;= 10<sup>18</sup></i>, <i>1&lt;= p &lt;= 10<sup>8</sup></i>)<br>

</p><h3>Output</h3>
<p>Exactly <i>C</i> lines, one for each test case:
 (<i>a<sub>m</sub></i> + <i>a<sub>m+1</sub></i> + <i>a<sub>m+2</sub></i> + ... + <i>a<sub>n</sub></i>) modulo <i>p</i>.

</p><h3>Example</h3>

<pre><b>Input:</b>
1
2
1 1
1 1
2 10 1000003

<b>Output:</b>
142
</pre>