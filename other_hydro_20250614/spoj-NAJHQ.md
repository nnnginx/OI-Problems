<p>Hazzat is a new guys in computer science.&nbsp; Now he read in 4<sup>rd</sup> semester. Recently he completed the course data structure. After finished data structure course he can realize that those are not enough for his. Every day he fall in a new (data structure) problem and want solve it, but those problem he can��t solve&nbsp; using his know data structure. He want to establish new data structure. But he always failed to establish it. Now help hazzat to establish a new data structure following problems.</p>
<p>Today Hazzat problem is-</p>
<p>Given a N size Array (arr[N]) initialize all the element value is exactly c.</p>
<p>see the pseudo</p>
<p>for(i=1;i&lt;=N;i++)</p>
<p>arr[i]=c;</p>
<p>Today Hazzat want to do 6 types of task.</p>
<p><strong>i)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong><strong>add&nbsp; exactly k value from array index u to v </strong></p>
<p>see the pseudo</p>
<p>for(i=u;i&lt;=v;i++)</p>
<p>arr[i]=arr[i]+k;<strong>&nbsp;</strong></p>
<p><strong>ii)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong><strong>minus exactly k value from array index u to v </strong></p>
<p>see the pseudo</p>
<p>for(i=u;i&lt;=v;i++)</p>
<p>arr[i]=arr[i]-k;<strong>&nbsp;</strong></p>
<p><strong>iii)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong><strong>add exactly k value only array index u</strong></p>
<p>see the pseudo</p>
<p>arr[u]=arr[u]+k;</p>
<p><strong>iv)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong><strong>minus exactly k value only array index u </strong></p>
<p>see the pseudo</p>
<p>arr[u]=arr[u]-k;<strong>&nbsp;</strong></p>
<p><strong>v)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong><strong>reset a array index u with k value</strong></p>
<p>see the pseudo</p>
<p>arr[u]= k;<strong>&nbsp;</strong></p>
<p><strong>vi)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong><strong>find the current value of array index u </strong></p>
<p>see the pseudo</p>
<p>print arr[u];</p>
<p>Here the array is 1 base index.</p>
<p><strong>Input:</strong></p>
<p>Input start with an integer number T(��10), which is number of test cases.</p>
<p>For each test case</p>
<p>First line given</p>
<p><strong>N</strong><strong> Q c</strong> where N is array size, Q number of queries and c is the initialize value of array.</p>
<p>Next Q line give the Hazzat task��s</p>
<p><strong>add u v k</strong> (add exactly k values from array index u to v)</p>
<p><strong>minus u v k </strong>(minus exactly k values from array index u to v)</p>
<p><strong>&nbsp;addin u k</strong> (add exactly k value only array index u)</p>
<p><strong>minusin u k</strong> (minus exactly k value only array index u)</p>
<p><strong>reset u k</strong> (reset a array index u with k value)</p>
<p><strong>find u</strong> (print current value of array index u)</p>
<p><strong>Constrains: </strong></p>
<ul>
<li><strong>T��10</strong></li>
<li><strong>1 �� N, Q ��10^5</strong></li>
<li><strong>1�� u �� v��N</strong></li>
<li><strong>0��c,k��10^9</strong></li>
</ul>
<p><strong>Output:</strong></p>
<p>For each case, Print ��Case #X�� where X is case number.</p>
<p>After Next line print value of array index u where hazzat want to know. (only for <strong>find u</strong> task)</p>
<p>There will be a blank line between two case.</p>
<p><strong>Sample:</strong></p>
<table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="258" valign="top">
<p>Input</p>
</td>
<td width="198" valign="top">
<p>Output</p>
</td>
</tr>
<tr>
<td width="258">
<p>2<br>10 3 3<br>find 4<br>add 3 7 3<br>find 5<br><br>10 10 3<br>find 4<br>add 3 7 2<br>find 6<br>minus 3 4 1<br>find 4<br>addin 4 5<br>find 4<br>minusin 4 2<br>find 4<br>find 10</p>
</td>
<td width="198">
<p>Case #1<br>3<br>6<br><br>Case #2<br>3<br>5<br>4<br>9<br>7<br>3</p>
</td>
</tr>
</tbody>
</table>
<p><br>Output number may be Negetive.<br>Data set is so huge. Use faster I/O</p>