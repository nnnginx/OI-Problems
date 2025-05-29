<p><span style="font-size: medium;">Hazzat is a new guys in computer science.&nbsp; Now he read in 4rd semester. Recently he completed the course data structure. After finished data structure course he can realize that those are not enough for his. Every day he fall in a new (data structure) problem and want solve it, but those problem he can¡¯t solve&nbsp; using his know data structure. He want to establish new data structure. But he always failed to establish it. Now help hazzat to establish a new data structure following problems.</span></p>
<p><span style="font-size: medium;">You will be given an array <strong>A</strong> of <strong>N</strong> integers. You need to answer <strong>M</strong> queries.<br> Each query is of the form <strong>V x y</strong>. </span></p>
<p><span style="font-size: medium;"><span><span><span>For each query, find the sum of  set S which is a sub set of array A index x to y and fully divisible by V.</span></span></span></span></p>
<p><span style="font-size: medium;">That means find sum of set S (subset of A), where A[i] is included in S if x ¡Ü i ¡Ü y and A[i]%V==0.</span></p>
<p><span style="font-size: medium;"><br></span></p>
<p><strong><span style="font-size: medium;">I</span><span style="font-size: medium;">nput:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span></strong></p>
<p><span style="font-size: medium;"> </span></p>
<p><span style="font-size: medium;">First&nbsp; line consists of a number T (1 ¡Ü T ¡Ü 5) test cases.</span></p>
<p><span style="font-size: medium;">For each case given two integer number&nbsp; N M,&nbsp; (1¡Ü N¡Ü 10^5, 1¡ÜM ¡Ü 2*10^5)</span></p>
<p><span style="font-size: medium;">Next line has N integers representing the elements of array A. 1¡ÜA[]¡Ü 10^6</span></p>
<p><span style="font-size: medium;">&nbsp;</span><span style="font-size: medium;">M lines follow, one per query.</span></p>
<p><span style="font-size: medium;">Each line has 3 integers V, x and y&nbsp; (1¡Ü V ¡Ü 1000 , 1¡Ü x ¡Ü y ¡ÜN)</span></p>
<p><span style="font-size: medium;"><br></span></p>
<p><span style="font-size: medium;"> </span></p>
<p><span style="font-size: medium;"><strong>Output: </strong></span></p>
<p><span style="font-size: medium;"> </span></p>
<p><span style="font-size: medium;">For each case print Case No and query answer.</span></p>
<p><span style="font-size: medium;">There will be a blank line between two cases.</span></p>
<p><span style="font-size: medium;"><br></span></p>
<p><span style="font-size: medium;"> </span></p>
<p><span style="font-size: medium;"><strong>Sample:</strong></span></p>
<p><span style="font-size: medium;"> </span></p>
<table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="258" valign="top">
<p><span style="font-size: medium;">Input</span></p>
</td>
<td width="198" valign="top">
<p><span style="font-size: medium;">Output</span></p>
</td>
</tr>
<tr>
<td width="258">
<p><span style="font-size: medium;">2</span><br> <span style="font-size: medium;">5 2</span><br> <span style="font-size: medium;">1 2 3 4 6</span><br> <span style="font-size: medium;">2 1 5</span><br> <span style="font-size: medium;">5 1 4</span><br> <span style="font-size: medium;">&nbsp;</span><br> <span style="font-size: medium;">5 2</span><br> <span style="font-size: medium;">2 3 5 3 7</span><br> <span style="font-size: medium;">3 2 4</span><br> <span style="font-size: medium;">5 1 5</span></p>
</td>
<td width="198" valign="top">
<p><span style="font-size: medium;">Case   #1</span><br><span style="font-size: medium;">12</span><br> <span style="font-size: medium;">0</span><br> <span style="font-size: medium;">&nbsp;</span><br> <span style="font-size: medium;">Case   #2</span><br> <span style="font-size: medium;">6</span><br> <span style="font-size: medium;">5</span></p>
</td>
</tr>
</tbody>
</table>
<p><span style="font-size: medium;"> </span></p>
<p><span style="font-size: medium;">&nbsp;</span></p>
<p><span style="font-size: medium;"> </span></p>
<p><span style="font-size: medium;">Hints:</span></p>
<p><span style="font-size: medium;"> </span></p>
<p><span style="font-size: medium;">Query 1:<br>In array index 1 to 5 the set S is {2,4,6} because those are fully divisible by 2. so sum is 12</span></p>
<p><span style="font-size: medium;">Query 2:<br>In array index 1 to 4&nbsp; the set S is {} because there are not any number which fully divisible by 5. so sum is 0<br> <br></span></p>
<p><span style="font-size: medium;"> </span></p>
<p><span style="font-size: medium;">Data set is so huge. Use faster I/O</span></p>