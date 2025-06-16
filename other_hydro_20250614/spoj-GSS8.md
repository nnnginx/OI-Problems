<p><span style="background-color: #ffffff;">You are given sequence A[0], A[1]...A[N - 1]. (0 &lt;= A[i] &lt; 2^32)</span></p>
<p><span style="background-color: #ffffff;">You are to perform Q operations:</span></p>
<p><span style="background-color: #ffffff;">1. <strong>I pos val</strong>, insert number <strong>val </strong>in sequence before element with index <strong>pos</strong>. (0 &lt;= val &lt; 2^32, if <strong>pos</strong>&nbsp;= <strong>current_length</strong>&nbsp;then you should add number to the end of the sequence)</span></p>
<p><span style="background-color: #ffffff;">2. <strong>D pos</strong>, delete element with index <strong>pos </strong>from sequence.</span></p>
<p><span style="background-color: #ffffff;">3. <strong>R pos val</strong>, replace element with idex <strong>pos </strong>by <strong>val</strong>. (0 &lt;= val &lt; 2^32)</span></p>
<p><span style="background-color: #ffffff;">4. <strong>Q l r k</strong>, answer ��&nbsp;A[i] * (i - l + 1)^k modulo 2^32, for l &lt;= i &lt;= r. (0 &lt;= k &lt;= 10)</span></p>
<h3><span style="background-color: #ffffff;">Input</span></h3>
<p style="text-align: justify;"><span style="color: #000020; font-size: x-small;"><span style="background-color: #f6f9e0;"><span style="font-size: small;"><span style="background-color: #ffffff;">The first line of the input contains an integer N (1 &lt;= N &lt;= 100000).</span></span></span></span></p>
<p style="text-align: justify;"><span style="color: #000020; font-size: x-small;"><span style="background-color: #f6f9e0;"><span style="font-size: small;"><span style="background-color: #ffffff;">The following line contains N integers, representing the starting sequence A[0]..A[N-1].</span></span></span></span></p>
<p style="text-align: justify;"><span style="color: #000020; font-size: x-small;"><span style="background-color: #f6f9e0;"><span style="font-size: small;"><span style="background-color: #ffffff;">The third line contains an integer Q (0 &lt;= Q &lt;= 100000).</span></span></span></span></p>
<p style="text-align: justify;"><span style="color: #000020; font-size: x-small;"><span style="background-color: #f6f9e0;"><span style="font-size: small;"><span style="background-color: #ffffff;">Next lines contains queries in given format.</span></span></span></span></p>
<h3><span style="background-color: #ffffff;">Output</span></h3>
<p><span style="background-color: #ffffff;"><span style="color: #000020; font-size: 13px; text-align: justify;">For each&nbsp;</span><strong>"Q"</strong><span style="color: #000020; font-size: 13px; text-align: justify;">&nbsp;operation, print an integer(one per line) as described above.</span></span></p>
<h3><span style="background-color: #ffffff;">Example</span></h3>
<pre><span style="background-color: #ffffff;"><strong>Input:</strong>
</span><div id="_mcePaste" style="position: absolute; left: -10000px; top: 147px; width: 1px; height: 1px; overflow: hidden;"><span style="background-color: #ffffff;">4</span></div><span style="background-color: #ffffff;">4
1 2 3 5
7
Q 0 2 0
I 3 4
Q 2 4 1
D 0
Q 0 3 1
R 1 2
Q 0 1 0</span></pre>
<pre><span style="background-color: #ffffff;"><strong>Output:</strong>
6
26
40
4</span></pre>