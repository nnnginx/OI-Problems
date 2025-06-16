<p><span style="font-size: medium;">Angel Luis is now getting math class. His teacher is teaching to him the XOR operation.</span></p>
<p><span style="font-size: medium;">0 XOR 0 = 0</span></p>
<p><span style="font-size: medium;">0 XOR 1 = 1</span></p>
<p><span style="font-size: medium;">1 XOR 0 = 1</span></p>
<p><span style="font-size: medium;">1 XOR 1 = 0</span></p>
<p><span style="font-size: medium;">When is a number with more than a bit it operation is made to all bits. The teacher write two number x,y (0&lt;=x&lt;=N and 0&lt;=y&lt;=N) and make the XOR operation betwen x and y, Angel Luis would like to know how many pairs x,y such x XOR y = 2<sup>z &nbsp; </sup>where z&gt;=0.</span></p>
<p><span style="font-size: medium;">See that for N = 3 :</span></p>
<p><span style="font-size: medium;">0 XOR 1 = 2<sup>0</sup></span></p>
<p><span style="font-size: medium;"><span style="font-size: medium;">0 XOR 2 = 2</span><sup>1</sup></span></p>
<p><span style="font-size: medium;"><span style="font-size: medium;">3 XOR 1 = 2</span><sup>1</sup></span></p>
<p><span style="font-size: medium;"><span style="font-size: medium;">2 XOR 3 = 2</span><sup>0</sup></span></p>
<p><span style="font-size: medium;">So there is 4 pairs.</span></p>
<p><span style="font-size: medium;">Given N you should return how many pair module 1000000007.</span></p>
<h3><span style="font-size: medium;">Input</span></h3>
<p><span style="font-size: medium;">First line a number t (number of cases) each t line will have a number N</span></p>
<p><span style="font-size: medium;">t&lt;=100</span></p>
<p><span style="font-size: medium;">N&lt;=1000000000000000 (10<sup>15</sup>).</span></p>
<h3><span style="font-size: medium;">Output</span></h3>
<p><span style="font-size: medium;">For each case a number of pair module 1000000007.</span></p>
<h3><span style="font-size: medium;">Example</span></h3>
<pre><span style="font-size: medium;"><strong>Input:</strong>
3
1</span></pre>
<pre><span style="font-size: medium;">2</span></pre>
<pre><span style="font-size: medium;">3
<strong>Output:</strong>
1</span></pre>
<pre><span style="font-size: medium;">2</span></pre>
<pre><span style="font-size: medium;">4</span></pre>