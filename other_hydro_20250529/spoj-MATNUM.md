<p>Problem statement is simple and straight forward . You will be given a non-negative integer <strong>P </strong>of length <strong>N </strong>and you need to check whether it's divisible by <strong>Q </strong>?</p>
<p>Integer <strong>P </strong>will be given in its decimal representation with <strong>P<sub>0</sub> </strong>as leftmost digit and <strong>P<sub>1</sub> </strong>as second digit from left !</p>
<p>Rest of the digit can be generated from the formula :</p>
<p><span style="white-space:pre"> </span><strong>P<sub>i</sub> = ( 4*P<sub>i-1</sub>&nbsp;+ P<sub>i-2</sub> ) modulo Q</strong> &nbsp; &nbsp; &nbsp;for&nbsp;<span style="white-space: pre;"> </span><strong>2 &lt;= i &lt;= N-1</strong></p>
<h3>Input</h3>
<p>The first line contains one integer <strong>T </strong>- denoting the number of test cases.</p>
<p><strong>T </strong>lines follow each containing four integers <strong>P<sub>0</sub> </strong>, <strong>P<sub>1</sub> </strong>, <strong>Q </strong>and <strong>N </strong>!</p>
<h3>Output</h3>
<p>For each testcase output <strong>YES </strong>if the corresponding integer is divisible by <strong>Q </strong>and <strong>NO </strong>otherwise.</p>
<h3>Constraints</h3>
<ul>
<li><strong>T &lt;= 100000</strong></li>
<li><strong>0 &lt; P<sub>0</sub> , P<sub>1</sub> , Q &lt; 10</strong></li>
<li><strong><span style="vertical-align: sub;">0 &lt; N &lt;= 10</span><span style="vertical-align: sub;"><sup>18</sup></span></strong></li>
</ul>
<h3>Example</h3>
<pre><strong>Input:</strong>
4
1 4 2 2
1 4 2 1
4 2 3 2
3 4 7 3

<strong>Output:</strong>
YES
NO
YES
NO</pre>

<h3>Explanation</h3>
<p>Value of <strong>P </strong>is <strong>14, 1, 42, 345 </strong>in respective cases !<strong>&nbsp;</strong></p>