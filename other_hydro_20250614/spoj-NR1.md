<p><span style="font-size: small;">Kapti and Balu are friends. Kapti is very good in math and is always saying that no one can challenge him in math. One day Balu decided to check Kapti that he is really good in math or he is just making fool.</span></p>
<p><span style="font-size: small;">Balu gave Kapti a polynomial of degree ��n��&nbsp; and ask Kapti to find constant term ��L�� if the polynomial was first expressed in Factorial Notation and then subjected to Forward Difference operator for ��k�� &nbsp;imes.</span></p>
<p><span style="font-size: small;">If &nbsp;&nbsp;&nbsp;&nbsp;</span></p>
<p><span style="font-size: small;"><em>&nbsp; &nbsp;f</em>(x)=a<sub>1</sub>x<sup>n</sup>&nbsp;+ a<sub>2</sub>x<sup>n-1</sup>&nbsp;+ ........... + a<sub>n</sub>x + l &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;<br> then its factorial notation will be:&nbsp;&nbsp;</span></p>
<p><span style="font-size: small;"><em>&nbsp; &nbsp;f</em><sub>FN</sub>(x)=A<sub>1</sub>[x]<sup>n</sup>&nbsp;+ A<sub>2</sub>[x]<sup>n-1</sup>&nbsp;+ .......... + A<sub>n</sub>[x] + L&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp;</span></p>
<p><span style="font-size: small;">Where&nbsp; </span></p>
<p><span style="font-size: small;">&nbsp; &nbsp;[x]<sup>n</sup>=x(x-1)(x-2)......(x-n+1)&nbsp;</span></p>
<p><span style="font-size: small;">And forward difference operator ��&nbsp;is just simple differentiation of &nbsp;<em>f</em><sub>FN</sub>(x).</span></p>
<p><span style="font-size: small;">For example&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;</span></p>
<p><span style="font-size: small;"><em>f</em>(x)=2x<sup>3</sup>&nbsp;- 3x<sup>2</sup>&nbsp;+ 3x - 10</span></p>
<p><span style="font-size: small;"><em>f</em><sub>FN</sub>(x)=2[x]<sup>3</sup>&nbsp;+ 3[x]<sup>2</sup>&nbsp;+ 2[x] - 10</span></p>
<p><span style="font-size: small;">��<em>f</em><sub>FN</sub>(x)=6[x]<sup>2</sup>&nbsp;+ 6[x] + 2&nbsp;&nbsp;here constant term L=2 and k=1;</span></p>
<p><span style="font-size: small;">Help kapti in proving himself that he is good in math.</span></p>
<h3>Input</h3>
<p><span style="font-size: small;">Input start with integer <strong>T(&lt;30) </strong>denoting the number of test cases.</span></p>
<p><span style="font-size: small;">Each test case will contains two lines,</span></p>
<p><span style="font-size: small;">First line contains <strong>n(&lt;=25)</strong> &amp; <strong>k(&lt;=n)</strong></span></p>
<p><span style="font-size: small;">Second line contains <strong>n+1</strong> integers <em>a<sub>1</sub>&nbsp;a<sub>2</sub>&nbsp;a<sub>3</sub>&nbsp;........ a<sub>n</sub>&nbsp;l , -50&lt;=a<sub>i</sub>&lt;=50</em></span></p>
<h3>Output</h3>
<p><span style="font-size: small;">For each test case print one line containing &nbsp;L.</span></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-size: xx-small;"><br></span></pre>
<pre><p><strong><span style="font-size: medium;">1</span></strong></p><span style="font-size: medium;">
</span><p><strong><span style="font-size: medium;">3  2</span></strong></p><span style="font-size: medium;">
</span><p><strong><span style="font-size: medium;">2 -3 3 -10</span></strong></p>

<strong>Output:</strong></pre>
<pre><span style="font-size: small;"><strong><span style="font-size: medium;">6</span></strong></span>
</pre>