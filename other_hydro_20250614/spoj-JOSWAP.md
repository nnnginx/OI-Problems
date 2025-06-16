<p><span style="color: #3e3f3a; font-size: 14px;"><span style="font-size: small;"><span style="font-family: tahoma, arial, helvetica, sans-serif;">You are given an array of size N. How many distinct arrays can you generate by swapping two numbers for exactly once? The two selected numbers can be equal but their positions in the array must be different.</span></span></span></p>
<h3>Input</h3>
<p><span style="color: #3e3f3a; font-size: 14px;"><span style="font-size: small;"><span style="font-family: tahoma, arial, helvetica, sans-serif;">The first line of the input contains a single integer T, denoting the number of test cases. Every test case starts with an integer N. The next line contains N integers, the numbers of the array.</span></span></span></p>
<h3>Output</h3>
<p><span style="color: #3e3f3a; font-size: 14px;"><span style="font-size: small;"><span style="font-family: tahoma, arial, helvetica, sans-serif;">For each tescase output the answer in a single line.</span></span></span></p>
<p>&nbsp;</p>
<h3><span style="color: #3e3f3a; font-size: 14px;"><span style="font-family: &quot;arial black&quot;, &quot;avant garde&quot;;">Constraints</span></span><span style="color: #3e3f3a; font-family: &quot;PT Sans&quot;; font-size: 14px;">:</span></h3>
<p style="box-sizing: border-box; margin: 0px 0px 10px; color: #3e3f3a; font-size: 14px;"><span style="font-size: small;"><span style="font-family: tahoma, arial, helvetica, sans-serif;">1 &lt;= T &lt;= 5</span></span></p>
<p style="box-sizing: border-box; margin: 0px 0px 10px; color: #3e3f3a; font-size: 14px;"><span style="font-size: small;"><span style="font-family: tahoma, arial, helvetica, sans-serif;">1 &lt;= Value of a number in the array &lt;= 100000</span></span></p>
<p style="box-sizing: border-box; margin: 0px 0px 10px; color: #3e3f3a; font-family: &quot;PT Sans&quot;; font-size: 14px;"><span style="color: #3e3f3a; font-size: 14px;"><span style="font-size: small;"><span style="font-family: tahoma, arial, helvetica, sans-serif;">2 &lt;= N &lt;= 100000</span></span></span></p>
<p style="box-sizing: border-box; margin: 0px 0px 10px; color: #3e3f3a; font-family: &quot;PT Sans&quot;; font-size: 14px;"><span style="color: #3e3f3a; font-family: &quot;PT Sans&quot;; font-size: 14px;"><br></span></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p><span style="color: #3e3f3a; font-family: &quot;Ubuntu Mono&quot;; font-size: 14px; white-space: pre;">1 <br></span><span style="color: #3e3f3a; font-family: &quot;Ubuntu Mono&quot;; font-size: 14px; white-space: pre;">5 <br></span><span style="color: #3e3f3a; font-family: &quot;Ubuntu Mono&quot;; font-size: 14px; white-space: pre;">2 3 2 3 3</span></p></pre>
<pre><strong>Output:</strong>
<span style="color: #3e3f3a; font-family: &quot;Ubuntu Mono&quot;; font-size: 14px; white-space: pre;">7</span></pre>
<pre><p style="box-sizing: border-box; margin: 0px 0px 10px; color: #3e3f3a; font-size: 11.9px;"><span style="font-size: small;">You can generate the following arrays:</span></p><span style="font-size: small;">
</span><p style="box-sizing: border-box; margin: 0px 0px 10px; color: #3e3f3a; font-size: 11.9px;"><span style="font-size: small;">2 3 2 3 3</span></p><span style="font-size: small;">
</span><p style="box-sizing: border-box; margin: 0px 0px 10px; color: #3e3f3a; font-size: 11.9px;"><span style="font-size: small;">2 2 3 3 3</span></p><span style="font-size: small;">
</span><p style="box-sizing: border-box; margin: 0px 0px 10px; color: #3e3f3a; font-size: 11.9px;"><span style="font-size: small;">2 3 3 2 3</span></p><span style="font-size: small;">
</span><p style="box-sizing: border-box; margin: 0px 0px 10px; color: #3e3f3a; font-size: 11.9px;"><span style="font-size: small;">2 3 3 3 2</span></p><span style="font-size: small;">
</span><p style="box-sizing: border-box; margin: 0px 0px 10px; color: #3e3f3a; font-size: 11.9px;"><span style="font-size: small;">3 2 2 3 3</span></p><span style="font-size: small;">
</span><p style="box-sizing: border-box; margin: 0px 0px 10px; color: #3e3f3a; font-size: 11.9px;"><span style="font-size: small;">3 3 2 2 3</span></p><span style="font-size: small;">
</span><p style="box-sizing: border-box; margin: 0px 0px 10px; color: #3e3f3a; font-size: 11.9px;"><span style="font-size: small;">3 3 2 3 2</span></p></pre>
<div><span style="color: #3e3f3a; font-family: &quot;PT Sans&quot;; font-size: 14px;"><br></span></div>