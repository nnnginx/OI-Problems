<p><span style="font-family: arial,helvetica,sans-serif;"><span style="font-size: small;"><span style="font-size: large;"><span style="text-decoration: underline;"><strong>Problem Statement</strong></span>:</span><br></span></span></p>
<p><span style="font-family: arial,helvetica,sans-serif;"> </span></p>
<pre><span style="font-family: arial,helvetica,sans-serif;"><span style="white-space: normal;"><p><span style="font-size: medium;">The number N is called <a href="../PSYCHON/" target="_blank"><strong>Psycho Number</strong></a> . Psycho Number is calculated as follows:</span></p><span style="font-size: medium;">
</span><p><span style="font-size: medium;">First, If we factorize N , then we have some prime and their power. Assume that, there are M powers. From M powers , you should count the number of even and odd powers. Then if the number of even power is strictly greater than odd power , then we call the number N is “<strong>Psycho Number</strong>”, otherwise the number N is call “<strong>Ordinary Number</strong>”.</span></p><span style="font-size: medium;">
</span><p><span style="font-size: medium;">As for example, if N = 67500 then prime factorization,&nbsp;</span></p><p><span style="font-size: medium;">67500 = 2<sup>2 </sup>x 3<sup>3 </sup>x 5<sup>4</sup>.&nbsp;</span></p><p><span style="font-size: medium;">Count even powers and odd powers . This number have 2 even power(2,4) and 1 odd power ( 3 ). Since even power 2 (2,4) is greater than odd power 1 (3), so the number 67500 is a Psycho Number.</span></p></span></span></pre>
<p><span style="font-family: arial,helvetica,sans-serif;"><span style="font-size: small;"><span style="font-size: medium;"><span style="font-size: small;"><span style="font-size: medium;"><span><span><span>Now, Given an integer <strong>K</strong>, your task is to find whether it is possible to form  a subset consisting of only psycho numbers that sum up to exactly <strong>K</strong>, or  not.</span></span></span></span></span></span></span></span></p>
<p><span style="font-family: arial,helvetica,sans-serif;"><span style="font-size: small;"><br><span style="font-size: large;"><span style="text-decoration: underline;"><strong>Input</strong></span>:</span><br><span style="font-size: medium;">The first line of the input contains an integer, <strong>T</strong> (1 ≤ <strong>T</strong> ≤ 2000) indicating the number of test cases. For each test case, two lines appear, the first one contains a number <strong>N</strong> (1 ≤ <strong>N</strong> ≤ 100), representing the length of the numbers . and <strong>K<span style="font-size: small;"><span style="font-size: medium;"><strong> </strong></span></span></strong><span style="font-size: small;"><span style="font-size: medium;">(1 ≤ <strong>K</strong> ≤ 10<sup>5</sup>)</span></span>. The second line of each test case contains the sequence of integers p<sub>1</sub>, p<sub>2</sub>, ..., p<sub>n</sub> (0 ≤ p<sub>i</sub> ≤ 1100).&nbsp; It's mixed with psycho number and ordinary number.</span><br><span style="font-size: medium;">&nbsp;</span></span></span></p>
<p><span style="font-family: arial,helvetica,sans-serif;"> </span></p>
<p><span style="font-family: arial,helvetica,sans-serif;"><span style="font-size: small;"><span style="font-size: large;"><strong><span style="text-decoration: underline;">Output</span>:</strong></span><br><span style="font-size: medium;">For each case print &nbsp;“<strong>Yes</strong>” if possible to make <strong>K</strong> . otherwise “<strong>No</strong>”.</span><br><br></span></span></p>
<p><span style="font-family: arial,helvetica,sans-serif;"> </span></p>
<pre><span style="white-space: normal;"><p><span style="font-family: arial,helvetica,sans-serif;"><span style="font-size: large;"><strong><span style="text-decoration: underline;">Sample Input/Output:</span></strong></span></span></p><span style="font-size: small;">
</span><table style="width: 653px; height: 94px;" border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="326" valign="top">
<p style="text-align: center;"><span style="font-family: arial,helvetica,sans-serif;"><span style="font-size: medium;"><strong>Sample Input</strong></span></span></p>
</td>
<td width="326" valign="top">
<p style="text-align: center;"><span style="font-family: arial,helvetica,sans-serif;"><span style="font-size: medium;"><strong>Sample Output</strong></span></span></p>
</td>
</tr>
<tr>
<td width="326" valign="top">
<p><strong><span style="font-size: medium;"><span style="font-family: arial,helvetica,sans-serif;">&nbsp; 3<br>&nbsp; 5 20<br>&nbsp; 4 5 12 20 16<br>&nbsp; 5 3<br>&nbsp; 3 5 9 2 7
&nbsp;<br>&nbsp; 3 24<br>&nbsp; 4 4 16</span><br>
</span></strong></p>

</td>
<td width="326" valign="top">
<p><strong><span style="font-size: medium;">&nbsp;<span style="font-family: arial,helvetica,sans-serif;">Yes</span></span></strong></p>
<p><strong><span style="font-size: medium;">&nbsp;<span style="font-family: arial,helvetica,sans-serif;">No</span></span></strong></p>
<p><strong><span style="font-size: medium;">&nbsp;<span style="font-family: arial,helvetica,sans-serif;">Yes</span><br></span></strong></p>
<p><strong>&nbsp;</strong></p>
</td>
</tr>
</tbody>
</table>
<span style="font-size: small;"> </span>
</span><span style="font-size: small;"><span style="font-family: 'comic sans ms', sans-serif;"><strong><span style="text-decoration: underline;"><br><span style="font-family: arial,helvetica,sans-serif;">Explanation </span></span></strong><span style="font-size: small;"><span style="font-family: arial,helvetica,sans-serif;">:   </span><br><span style="font-family: arial,helvetica,sans-serif;">   <strong><span style="text-decoration: underline;">1st test case</span></strong> : psycho numbers : </span></span></span></span><span style="font-family: arial,helvetica,sans-serif;"><span style="font-size: small;">4 and 16 .<br>       possible number: 4, 16 and 20 (4+16). <br>       k is 20 so you can make this number .<br>   <strong><span style="text-decoration: underline;">2nd test case</span></strong> : psycho numbers : only 9<br>      k is 3 but it's not possible to make subset of psycho numbers which sum is equal to k . <br>   <strong><span style="text-decoration: underline;">3rd test case</span></strong> : psycho numbers : 4 4 16<br>     possible number  : 4 , 16 , 20(16+4) and 24 (16+4+4)<br>      k is 24 so you can make this number .<br><br>Note : 0 and 1 is not a psycho number .<br><pre><span style="white-space: normal;"><pre><span style="font-family: arial,helvetica,sans-serif;"><span style="font-size: small;"><span style="font-family: comic sans ms,sans-serif;">Psycho 1 : <strong><a title="Psycho" href="../PSYCHON/" target="_blank">Psycho</a></strong><br>Psycho 2 : </span></span></span><span style="font-family: comic sans ms,sans-serif;"><span style="font-size: small;"><span style="white-space: normal;"><a title="Psycho Function" href="../PSYCHO2/" target="_blank"><strong>Psycho Function</strong></a></span></span></span><span style="font-family: arial,helvetica,sans-serif;"><span style="font-size: small;"> </span></span>
</pre>
</span></pre>
</span></span><span style="white-space: normal;">
<pre><span style="font-size: medium;"><span style="white-space: normal;"><hr>
</span></span><span style="font-family: arial,helvetica,sans-serif;"><span style="font-size: medium;"><span style="white-space: normal;"><span style="font-size: small;"><strong><span style="text-decoration: underline;">Problem setter</span>:&nbsp;&nbsp; Shipu Ahamed, Dept. of CSE</strong></span></span></span><span style="font-size: small;"><strong><em><br>Bangladesh University of Business and Technology (BUBT)</em></strong></span></span><span style="font-size: small;"><span style="white-space: normal;"><span style="font-family: arial,helvetica,sans-serif;"><span style="font-size: small;"> </span></span><br></span></span><span style="font-size: small;"><span style="white-space: normal;">
<pre><span style="white-space: normal;">
</span></pre>
</span></span></pre>
</span></pre>