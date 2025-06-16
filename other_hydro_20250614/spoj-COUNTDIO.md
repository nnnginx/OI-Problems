<p>Given a positive integer <em><strong>M</strong></em> and <em><strong>N</strong></em> positive integers <em><strong>a<sub>1</sub>, a<sub>2</sub>, ..., a<sub>N</sub></strong></em>. Count the number of non-negative integer tuples <strong><em>(x<sub>1</sub>, x<sub>2</sub>, ..., x<sub>N</sub>)&nbsp;</em></strong>such that:</p>
<p><em><strong>a<sub>1</sub> * x<sub>1</sub> + a<sub>2</sub>&nbsp;* x<sub>2</sub> + ... + a<sub>N</sub> * x<sub>N</sub> = M</strong></em></p>
<h3>Input</h3>
<p>- The first line contains two integers <em><strong>N</strong></em> and <em><strong>M</strong></em>.</p>
<p>- The second line contains <em><strong>N</strong></em> integers <em><strong>a<sub>1</sub>, a<sub>2</sub>, ..., a<sub>N</sub></strong></em> respectively.</p>
<h3>Output</h3>
<p>- Output only one integer, the number of asked tuples modulo&nbsp;<em><strong>998244353</strong></em>.</p>
<h3>Constrains</h3>
<ul>
<li>1 ≤ <em>N</em> ≤ 60 000</li>
<li>1 ≤ <em>M</em> ≤ 10<sup>18</sup></li>
<li>1 ≤ <em>a<sub>i</sub></em> ≤ 60 000</li>
<li> 1 ≤ <em>a<sub>1</sub> + a<sub>2</sub> + ... + a<sub>N</sub></em> ≤ 60 000</li>
</ul>
<h3>Example</h3>
<h4>Input:</h4>
<pre>3 10
3 2 5</pre>
<h4>Output:</h4>
<pre>4</pre>
<h4>Input:</h4>
<pre>5 100000
1 3 4 6 1000</pre>
<h4>Output:</h4>
<pre>865762992</pre>
<h3>Note</h3>
<ul>
<li>My solution runs in less than 0.8s for each input file, 6.3s in total.</li>
</ul>