<p>Your task is to calculate a^(b^(exp))</p>
<p>a:provided in input,10^5=&gt;a&gt;=0</p>
<p>b:provided in input,10^5=&gt;b&gt;=0</p>
<p>exp=(nC0)^2 + (nC1)^2 + (nC2)^2 + ......+(nCn)^2</p>
<p>n:provided in input,10^5=&gt;n&gt;=0</p>
<p><strong>Note: The Output for 0^0 should be 1.</strong></p>
<p>nCr denotes n choose r.</p>
<p>As the answer can be too large , you need to output modulo 10^9+7.</p>
<h3>Input</h3>
<p>The first line of each input file contains number of test cases t(t&lt;=1000).</p>
<p>Then follow a new line.</p>
<p>Then follow t lines,each conating 3 integers,(i.e a b n &nbsp;in order) each of them seperated by a space.</p>
<h3>Output</h3>
<p>Output Contains t lines,ith line conatins the answer of the ith test case.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1</pre>
<pre>1 1 1

<strong>Output:</strong>
1</pre>
<pre><strong>Explanation: </strong>In First test case, the Value of exp is 2, value of 1^(1^2) is 1,so output is 1.</pre>
<pre><strong>Note: First try out the tutorial version where limits are low. <a href="../../problems/POWRTU/">POWRTU</a></strong></pre>
<p><a href="../../problems/INTRO/">Click here to see my set of problems at Spoj.</a></p>