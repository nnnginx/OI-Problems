<p>FIBONACCI is the recursive sequence that is given by: F(n)=F(n-1)+F(n-2) with F(0)=0 and F(1)=1<br>In this problem we define FIBOSQRT that is given by: Fs(n)=Fs(n-1)+Fs(n-2)+2*SQRT(3+Fs(n-1)*Fs(n-2)) with Fs(0) and Fs(1) are given in the input file.<br> It's guaranteed that SQRT(3+Fs(n-1)*Fs(n-2)) is always an integer.&nbsp;<img title="Wink" src="../../gfx/jscripts/tiny_mce/plugins/emotions/img/smiley-wink.gif" border="0" alt="Wink">&nbsp;I've proved it by math theorem.</p>
<p>Now your task is to find Fs(n)<br>Since the number can be Big you have to find the result mod M.</p>
<h3>Input</h3>
<p>The first line is an integer T(1 �� <strong>T</strong> �� 111,111), denoting the number of test cases. Then, T test cases follow.</p>
<p>For each test case, there are four integers <strong>Fs(0)</strong>,<strong>Fs(1)</strong>(1 �� Fs(0)&nbsp;�� Fs(1) &lt; 10<sup>6</sup>),&nbsp;<strong>M</strong>(1 �� <strong>M</strong>&nbsp;&lt; 10<sup>9</sup>), and <strong>n</strong>(0&nbsp;�� <strong>n</strong>&nbsp;&lt; 10<sup>18</sup>) written in one line, separated by space.</p>
<h3>Output</h3>
<p>For each test case, output Fs(<strong>n</strong>) mod <strong>M</strong>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre>2</pre>
<pre>1 1 10 5</pre>
<pre>2 3 100 6

<strong>Output:</strong></pre>
<pre>4</pre>
<pre>82</pre>
<pre><span style="font-weight: bold; "><br></span></pre>
<pre><span style="font-weight: bold; ">Explanation:</span></pre>
<pre>Case #1:</pre>
<ul>
<li>Fs(0)=1</li>
<li>Fs(1)=1</li>
<li>Fs(2)=1+1+2*SQRT(3+1*1)=6</li>
<li>Fs(3)=6+1+2*SQRT(3+6*1)=13</li>
<li>Fs(4)=13+6+2*SQRT(3+13*6)=37</li>
<li>Fs(5)=37+13+2*SQRT(3+37*13)=94</li>
</ul>
<p><span style="white-space: pre;"> <span style="white-space: pre;"> </span></span>The answer is: 94 mod 10 = <strong>4</strong>.</p>
<pre>Case #2:</pre>
<ul style="white-space: normal; ">
<li>Fs(0)=2</li>
<li>Fs(1)=3</li>
<li>Fs(2)=3+2+2*SQRT(3+3*2)=11</li>
<li>Fs(3)=11+3+2*SQRT(3+11*3)=26</li>
<li>Fs(4)=26+11+2*SQRT(3+26*11)=71</li>
<li>Fs(5)=71+26+2*SQRT(3+71*26)=183</li>
<li>Fs(6)=183+71+2*SQRT(3+183*71)=482</li>
</ul>
<p><span style="white-space: normal;">&nbsp;<span style="white-space: pre;"> </span></span><span style="white-space: normal;">The answer is: 482 mod 100 = </span><strong>82</strong><span style="white-space: normal;">.</span></p>
<pre><span style="font-weight: bold;">Input File:</span></pre>
<pre>File #1: More than 100,000 random test cases (test your program speed <img title="Laughing" src="../../gfx/jscripts/tiny_mce/plugins/emotions/img/smiley-laughing.gif" border="0" alt="Laughing">)</pre>
<pre>File #2: Less than 10 test cases (tricky test cases that might give you WA <img title="Tongue out" src="../../gfx/jscripts/tiny_mce/plugins/emotions/img/smiley-tongue-out.gif" border="0" alt="Tongue out">)</pre>
<p>&nbsp;</p>
<p><span style="color: #339966;"><span style="color: #339966;"><strong><span style="text-decoration: underline;">Time Limit ��&nbsp;8*(My Program Top Speed)</span></strong></span></span></p>
<p>&nbsp;</p>
<p style="text-align: center;"><strong><strong><span style="font-size: small;">Warning: large Input/Output data, be careful with certain languages</span></strong></strong></p>
<p style="text-align: center;"><strong><br></strong></p>
<p><strong>See also:</strong> <a title="TJANDRA" href="../TJANDRA/" target="_blank">Another problem added by Tjandra Satria Gunawan</a></p>