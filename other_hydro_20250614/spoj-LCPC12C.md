<pre><strong><span style="white-space: normal;">Description</span><br></strong><span style="white-space: normal;">
<p>Johnny loves to listen to music so much. Each day he decides to add, delete or listen to a music track on his laptop by doing one of the following operations:</p>
<ol>
<li>Download a new track.</li>
<li>Delete the last downloaded track that is not deleted already.</li>
<li>Listen to the shortest track that is already on his laptop.</li>
</ol>
<p>Each test case Johnny starts with an empty collection of tracks, at day &nbsp;Johnny decides which action to be taken depending on the value of <strong><em>R[i]</em></strong> % 3. if <strong><em>R[i]</em></strong> % 3 = 0 he listens to the shortest track on his laptop, if <strong><em>R[i]</em></strong> % 3 = 1 he deletes the last downloaded track that is not deleted already, if <strong><em>R[i]</em></strong> %3 = 2 he downloads a new track whose length is <strong><em>R[i]</em></strong> minutes. Your task is to compute the total number of minutes Johnny spends listening to music.</p>
<p>To keep the input small, it will be codified in the following way. You will be given an array <strong><em>h</em></strong>. Use the following pseudo-code on <strong><em>h</em></strong> to generate an array <strong><em>R</em></strong>.</p>
<ul>
<li>input array:<strong><em> h</em></strong></li>
<li>output array: <strong><em>R</em></strong> (of size <strong><em>n</em></strong>)</li>
<li><strong><em>j</em></strong> := 0</li>
<li><strong><em>m</em></strong> := size of <strong><em>h</em></strong></li>
<li>for <strong><em>i</em></strong> := 0 to <strong><em>n</em></strong>-1
<ul>
<li><strong><em>R[i]</em></strong> := <strong><em>h[j]</em></strong></li>
<li><strong><em>s</em></strong> := (<strong><em>j</em></strong>+1)%<strong><em>m</em></strong></li>
<li><strong><em>h[j]</em></strong> := ( ( <strong><em>h[j]</em></strong> ^ <strong><em>h[s]</em></strong> ) + 13 ) % 835454957</li>
<li><strong><em>j</em></strong> := <strong><em>s</em></strong></li>
</ul>
</li>
</ul>
<p>This code, along with the constraints, ensures that the length of each track is between 0 and 835454956, inclusive. In the above code, % is the modulus operator and ^ is the bitwise XOR binary operator. If x and y are integers, (x ^ y) represents the bitwise XOR operation on them in C/C++ and Java.</p>
<h2>Input Format</h2>
<p>Input will start with <strong><em>T </em></strong>number of test cases. Each test case will consist of 2 lines the first line starts with 0 &lt; <strong><em>n </em></strong>&lt;= 10,000,000 (size of array <strong><em>R</em></strong>), 0 &lt; <strong><em>m</em></strong> &lt;= 50 (size of array <strong><em>h</em></strong>). The second line will contain <strong><em>M </em></strong>numbers 0 &lt;= <strong><em>h[i]</em></strong> &lt;= 835454956 which are the elements of array <strong><em>h</em></strong>.</p>
<h2>Output Format</h2>
<p>For each test case, output the result using the following format:</p>
<p><strong><em>k. S&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em></strong></p>
<p>Where <strong><em>k </em></strong>is the test case number (starting at 1), a single period, a single space, and <strong><em>S</em></strong> is the total time in minutes spent by Johnny listening to music.</p>
<table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="284" valign="top">
<h2>Sample Input</h2>
</td>
<td width="284" valign="top">
<h2>Sample Output</h2>
</td>
</tr>
<tr>
<td width="284" valign="top">
<p>2</p>
<p>6 6</p>
<p>8 5 2 4 8 9</p>
<p>10 4</p>
<p>9 4 3 10</p>
</td>
<td width="284" valign="top">
<p>1. 5</p>
<p>2. 52</p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p></span></pre>