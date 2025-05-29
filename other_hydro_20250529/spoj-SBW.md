<pre><br><span style="white-space: normal;"><p style="margin-bottom: 0in; text-align: center;"><span style="font-size: medium;"><strong>&nbsp;Super Borboleta World</strong></span></p>
<p style="margin-bottom: 0in; text-align: left;"><strong>The input/output were broken, I've fixed it and rejudged all submissions.&nbsp;</strong></p><p style="margin-bottom: 0in; text-align: left;">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">Raphaell is a well-known programmer who created the biggest game development company in the world, BGM (Boboleta's GameMaker). As recently one of its game �C S.B.W (Super Borboleta's World) - has became very popular, Raphaell decided </span></span><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">to</span></span><span style="font-family: Arial, sans-serif;"><span style="font-size: small;"> make an online version of S.B.W's game. In order to do this he'll expose the source code and the mechanism of that game so anyone is able to improve it.</span></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;"> At first the game is made of three main operations in which the user is able to call as much as necessary. As the game is composed by K arrays of lists where each list has at most N integers on it, the three operations can be described in the following way:</span></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">- Operation &lt;2&gt; &lt;x&gt; &lt;y&gt;: Insert the integer &lt;y&gt; to the end of the &lt;x&gt;-th list.</span></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">- Operation &lt;1&gt; &lt;x&gt; &lt;y&gt;: Clean every list whose index lie on the range between &lt;x&gt; and &lt;y&gt; (inclusive).</span></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">- Operation &lt;0&gt; &lt;x&gt; &lt;y&gt;: In each list between &lt;x&gt; and &lt;y&gt; calculate all the possible consecutive XOR sum's, where XOR stands for the operation Exclusive OR, and return the maximum value of all possible XOR sum's.</span></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;"> Raphaell has access to the original pseudocode which is given bellow:</span></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<pre style="text-align: justify;"><span style="font-size: medium;"><span style="color: #000000;">m &lt;- array( array() )</span>

<span style="color: #000000;"><span style="color: #0033cc;"><strong>def</strong></span> insert(x,y):</span>
<span style="color: #000000;">        insert y to m[x]</span>

<span style="color: #000000;"><span style="color: #0033cc;"><strong>def</strong></span> clear(x,y):</span>
<span style="color: #000000;">        <span style="color: #0033cc;"><strong>for</strong></span> i&lt;-x to y:</span>
<span style="color: #000000;">                clear m[i]</span>

<span style="color: #000000;"><span style="color: #0033cc;"><strong>def</strong></span> max_xor(x,y):</span>
<span style="color: #000000;">        best &lt;- 0</span>
<span style="color: #000000;">        <span style="color: #0033cc;"><strong>for</strong></span> i&lt;-0 to sizeOf m[x]:</span>
<span style="color: #000000;">                sum_xor &lt;- 0</span>
<span style="color: #000000;">                <span style="color: #0033cc;"><strong>for</strong></span> j&lt;-i to sizeOf m[x]:</span>
<span style="color: #000000;">                        sum_xor &lt;- sum_xor (xor) m[x][j]</span>
<span style="color: #000000;">                        best &lt;- <span style="color: #00aaaa;">max</span>(best,sum_xor)</span>
<span style="color: #000000;">        <span style="color: #0033cc;"><strong>if</strong></span> x &lt; y:</span>
<span style="color: #000000;">                best &lt;- <span style="color: #00aaaa;">max</span>(best, max_xor(x+1,y))</span>
<span style="color: #000000;">        <span style="color: #0033cc;"><strong>return</strong></span> best</span></span></pre>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">This implementation was efficient to the offline version of the game. However, as the online version may receive a thousands of players at once, it's necessary many optimizations to run the game properly. Even though his friend has already tried really hard to figure a way to improve the performance, he hasn't got any good results till now.</span></span>&nbsp;</p>
<p style="margin-bottom: 0in; text-align: center;"><strong>Input</strong></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: medium;"> </span></span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">The input </span></span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">contains several test cases. A test case begins with a line containing </span></span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">an</span></span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;"> integer </span></span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">Q</span></span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;"> (1 </span></span></span><span style="color: #000020;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">��</span></span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;"> </span></span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">Q</span></span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;"> </span></span></span><span style="color: #000020;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">��</span></span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;"> 10</span></span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">^</span></span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">5</span></span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">), </span></span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">where Q represents the number of operations that are going to be performed. Then follow Q lines, each containing an operation. </span></span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;"> </span></span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">All the operations are as described above:</span></span></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">- </span></span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">0 x y: </span></span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">In each list between </span></span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">x</span></span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;"> and y calculate all the possible consecutive XOR sum's </span></span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">and return the maximum possible value.</span></span></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">-  1 x y: </span></span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">Clean every list whose index lie on the range between x and y</span></span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;"> </span></span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">i</span></span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">nclusive.</span></span></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">-  2 x y: </span></span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">Insert the integer y to the end of the x-th list.</span></span></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;"> </span></span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">Both x and y in every operation will never exceed </span></span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">10^14</span></span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">. The last test case is followed by a line containing a single 0.</span></span></span></p>
<p style="margin-bottom: 0in; text-align: center;"><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: medium;"><strong>Output</strong></span></span></span></p>
<p style="margin-bottom: 0in;" align="CENTER">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-size: small;"><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"> For each </span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;">query &lt;0&gt; &lt;x&gt; &lt;y&gt; print </span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;">a line containing</span></span><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"> a single integer representing the maximum possible XOR as described above.</span></span></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in; text-align: center;"><span style="color: #333333;"><span style="font-family: Arial, sans-serif;"><span style="font-size: medium;"><strong>Example</strong></span></span></span></p>
<table style="width: 140px;" border="0" cellspacing="0" cellpadding="4">
<colgroup><col width="65"> <col width="57"> </colgroup> 
<tbody>
<tr valign="TOP">
<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0.04in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in;" width="65">
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: x-small;">Input</span></span></p>
</td>
<td style="border: 1px solid #000000; padding: 0.04in;" width="57">
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: x-small;">Output</span></span></p>
</td>
</tr>
<tr valign="TOP">
<td style="border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in;" width="65" height="84">
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: x-small;">14</span></span></p>
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: x-small;">2 			2 1</span></span></p>
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: x-small;">2 			2 2</span></span></p>
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: x-small;">2 			2 1</span></span></p>
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: x-small;">2 			2 1</span></span></p>
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: x-small;">2 			2 2</span></span></p>
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: x-small;">2 			3 1</span></span></p>
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: x-small;">2 			3 2</span></span></p>
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: x-small;">2 			3 7</span></span></p>
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: x-small;">0 			1 2</span></span></p>
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: x-small;">0 			2 3</span></span></p>
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: x-small;">1 			3 3</span></span></p>
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: x-small;">0 			1 3</span></span></p>
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: x-small;">1 			1 3</span></span></p>
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: x-small;">0 			1 3</span></span></p>
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: x-small;">0</span></span></p>
</td>
<td style="border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in;" width="57">
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: x-small;">3</span></span></p>
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: x-small;">7</span></span></p>
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: x-small;">3</span></span></p>
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: x-small;">0</span></span></p>
</td>
</tr>
</tbody>
</table>
<p style="margin-bottom: 0in;" align="LEFT">&nbsp;</p>
</span></pre>