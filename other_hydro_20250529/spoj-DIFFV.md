<p style="font-family: Arial, sans-serif; margin: 7px 0px 0px; padding: 0px; font-size: 12px; line-height: 1.5em; color: #444444; text-align: justify;"><span style="line-height: 1.5em;">You are given set of&nbsp;</span><strong>N</strong><span style="line-height: 1.5em;">&nbsp;vectors, each vector consists of&nbsp;</span><strong>K</strong><span style="line-height: 1.5em;">&nbsp;integers. Vector ex equals ey&nbsp;</span><strong>iff&nbsp;</strong><span style="line-height: 1.5em;">there exist function bijection&nbsp;</span><strong>f</strong><span style="line-height: 1.5em;">&nbsp;and integer&nbsp;</span><strong>r</strong><span style="line-height: 1.5em;">, such that ex[i] = f( ey[(i+r)%K] ), for each i in range [0, K&gt; Eg. (1, 2, 2, 3) == (22, 3, 4, 22), with r=2 and f(22)=2, f(3)=3 and f(4)=1. But (22,3,22,4) is not equal to (1, 2, 2, 3).</span></p>
<p style="font-family: Arial, sans-serif; margin: 7px 0px 0px; padding: 0px; font-size: 12px; line-height: 1.5em; color: #444444; text-align: justify;">How many different vectors are there in set of N given vectors ?</p>
<p style="font-family: Arial, sans-serif; margin: 7px 0px 0px; padding: 0px; font-size: 12px; line-height: 1.5em; color: #444444; text-align: justify;"><span style="line-height: 1.5em;">Constraints :</span></p>
<p style="font-family: Arial, sans-serif; margin: 7px 0px 0px; padding: 0px; font-size: 12px; line-height: 1.5em; color: #444444; text-align: justify;">n &lt;= 10000</p>
<p style="font-family: Arial, sans-serif; margin: 7px 0px 0px; padding: 0px; font-size: 12px; line-height: 1.5em; color: #444444; text-align: justify;">k &lt;= 100</p>
<p style="font-family: Arial, sans-serif; margin: 7px 0px 0px; padding: 0px; font-size: 12px; line-height: 1.5em; color: #444444; text-align: justify;">vector values are from range [0, 10^9]</p>
<h3>Input</h3>
<p><span style="color: #444444; font-family: Arial, sans-serif; font-size: 12px; line-height: 18px; text-align: justify;">First number contains T (T &lt;= 10), number of test cases. Each test cases consists of following. First line consists of N and K. N lines follows, the i-th containing K integers describing i-th vector.</span></p>
<h3>Output</h3>
<p><span style="color: #444444; font-family: Arial, sans-serif; font-size: 12px; line-height: 18px; text-align: justify;">Output one number, number of different vectors.</span></p>
<pre><strong>Input:<pre style="font-family: Arial, Helvetica, sans-serif; margin: 0px; padding: 0px; color: #444444; font-size: 12px; text-align: justify;">2
3 4
22 3 4 22
1 2 2 3
22 3 22 4
5 5
3 3 3 0 3
8 4 4 4 0
1 1 1 1 1
1 1 8 6 1
1 3 3 3 5
</pre>
</strong><strong>Output:</strong></pre>
<pre>2</pre>
<pre>3</pre>