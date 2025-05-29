<p><span style="font-family: comic sans ms,sans-serif;"><span style="font-size: large;"><strong><span style="text-decoration: underline;">Problem Statement:</span></strong></span></span></p>
<pre><span style="white-space: normal;"><p><span style="font-family: arial,helvetica,sans-serif;"><span style="font-size: medium;">The number N is called ¡°<a title="Psycho Number" href="../PSYCHON/" target="_blank"><strong>Psycho Number</strong></a>¡± . Psycho Number is calculated as follows:</span></span></p><span style="font-size: medium;">
</span><p><span style="font-family: arial,helvetica,sans-serif;"><span style="font-size: medium;">First, If we factorize N , then we have some prime and their power. Assume that, there are M powers. From M powers , you should count the number of even and odd powers. Then if the number of even power is strictly greater than odd power , then we call the number N is ¡°<strong>Psycho Number</strong>¡±, otherwise the number N is call ¡°<strong>Ordinary Number</strong>¡±.</span></span></p><span style="font-size: medium;">
</span><p><span style="font-family: arial,helvetica,sans-serif;"><span style="font-size: medium;">As for example, if N = 67500 then prime factorization,&nbsp;</span></span></p><p><span style="font-family: comic sans ms,sans-serif;"><span style="font-size: medium;">67500 = 2<sup>2 </sup>x 3<sup>3 </sup>x 5<sup>4</sup>.&nbsp;</span></span></p><p><span style="font-family: arial,helvetica,sans-serif;"><span style="font-size: medium;">Count even powers and odd powers . This number have 2 even power(2,4) and 1 odd power ( 3 ). Since even power 2 (2,4) is greater than odd power 1 (3), so the number 67500 is a Psycho Number.</span></span></p><!-- P { margin-bottom: 0.08in; direction: ltr; color: rgb(0, 0, 0); widows: 2; orphans: 2; }A:link {  } -->
<p style="margin-bottom: 0.14in;"><span style="font-family: arial,helvetica,sans-serif;"><span style="font-size: medium;">Now , You have to find the psycho number or Ordinary Number of the following function:</span></span></p><span style="font-family: comic sans ms,sans-serif;"><span style="font-size: medium;">
</span></span>
<pre><p style="margin-bottom: 0.14in;"><span style="font-size: medium;">bool isPsycho( long long K, long long b, long long p)</span>
<span style="font-size: medium;">{</span><span style="font-family: comic sans ms,sans-serif;">&nbsp;</span><span style="font-size: medium;">&nbsp;</span><span style="font-size: medium;"><br></span></p><p style="margin-bottom: 0.14in;"><span style="font-size: medium;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; N = numberoftrailingzeros ( K ! ) * lastdigit ( b</span><sup><span style="font-size: small;">p</span></sup><sup> </sup><span style="font-size: medium;">) ;</span><span style="font-size: medium;"> <br></span></p><p style="margin-bottom: 0.14in;"><span style="font-size: medium;">       if( N == psychonumber )</span></p><p style="margin-bottom: 0.14in;"><span style="font-size: medium;">            &nbsp;return true;</span><span style="font-family: comic sans ms,sans-serif;">&nbsp;</span><span style="font-size: medium;"><br></span></p><p style="margin-bottom: 0.14in;"><span style="font-size: medium;">      &nbsp;else <br></span></p><p style="margin-bottom: 0.14in;"><span style="font-size: medium;">            return false;</span>
</p><p style="margin-bottom: 0.14in"><span style="font-size: medium;">}</span>
</p></pre>
<span style="font-family: arial,helvetica,sans-serif;"><span style="font-size: medium;">For example , if  k = 10 , b= 12 , p = 1 then the N is 4 and it's a psycho number.<br>10 ! = 3628800 , number of trailingzeros is 2.<br>12<sup>1</sup><sup> </sup>= 12 , last digit is 2.<br>so N = 4 then 4 = 2<sup>2 </sup>. even power is greater than odd power, so the number 4 is a Psycho Number.</span></span>
<p>&nbsp;</p>
<p><span style="font-family: comic sans ms,sans-serif;"><span style="font-size: large;"><strong><span style="text-decoration: underline;">Input:</span></strong></span></span></p>
<!-- P { margin-bottom: 0.08in; direction: ltr; color: rgb(0, 0, 10); line-height: 115%; widows: 2; orphans: 2; }P.western { font-family: "Calibri",serif; font-size: 11pt; }P.cjk { font-family: "DejaVu Sans"; font-size: 11pt; }P.ctl { font-family: "Calibri"; font-size: 11pt; }A:link {  } -->
<p style="margin-bottom: 0.14in;"><span style="font-family: arial,helvetica,sans-serif;"><span style="font-size: medium;">An integer </span><span style="font-size: medium;"><strong>T</strong></span><span style="font-size: medium;"> (1&lt;= </span><span style="font-size: medium;"><strong>T</strong></span><span style="font-size: medium;"> &lt;=</span><span style="font-size: medium;">10<sup>5</sup></span><span style="font-size: medium;">) denoting the number of test cases followed by T lines. Each line containing <strong>K</strong> (1&lt;= <strong>K</strong> &lt;=4*10</span><span style="font-size: medium;"><sup><span style="font-size: small;">6</span></sup><span style="font-size: small;">), <span style="font-size: medium;"><strong>b</strong> (0&lt;= <strong>b</strong> &lt;=10</span></span><span style="font-family: arial,helvetica,sans-serif;"><span style="font-size: medium;"><sup>4</sup>), and <strong>p</strong> (0&lt;= <strong>p</strong> &lt;=10<sup>17</sup>).</span></span></span></span></p>
<p><span style="font-family: comic sans ms,sans-serif;"><span style="font-size: large;"><strong><span style="text-decoration: underline;">Output:</span></strong></span></span></p>
<p><span style="font-family: arial,helvetica,sans-serif;"><span style="font-size: medium;">For each case print &nbsp;¡°<strong>Psycho Number</strong>¡± or ¡°<strong>Ordinary Number</strong>¡±.</span></span></p>
<p>&nbsp;</p>
<p><span style="font-family: comic sans ms,sans-serif;"><span style="font-size: large;"><strong><span style="text-decoration: underline;">Sample Input/Output:</span></strong></span></span></p>
<table style="width: 653px; height: 94px;" border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="326" valign="top">
<p style="text-align: center;"><span style="font-family: comic sans ms,sans-serif;"><span style="font-size: medium;"><strong>Sample Input</strong></span></span></p>
</td>
<td width="326" valign="top">
<p style="text-align: center;"><span style="font-family: comic sans ms,sans-serif;"><span style="font-size: medium;"><strong>Sample Output</strong></span></span></p>
</td>
</tr>
<tr>
<td width="326" valign="top">
<p><strong>&nbsp;<span style="font-family: comic sans ms,sans-serif;"><span style="font-size: medium;">2</span></span></strong></p>
<span style="font-family: comic sans ms,sans-serif;"><span style="font-size: medium;"> </span></span>
<p><span style="font-family: comic sans ms,sans-serif;"><span style="font-size: medium;"><strong>&nbsp;5&nbsp; 2&nbsp; 5<br></strong></span></span></p>
<span style="font-family: comic sans ms,sans-serif;"><span style="font-size: medium;"> </span></span>
<p><span style="font-family: comic sans ms,sans-serif;"><span style="font-size: medium;"><strong>&nbsp;10&nbsp; 12&nbsp; 1<br></strong></span></span></p>
</td>
<td width="326" valign="top">
<p><span style="font-family: comic sans ms,sans-serif;"><span style="font-size: medium;"><strong>&nbsp;Ordinary Number</strong></span></span></p>
<span style="font-family: comic sans ms,sans-serif;"><span style="font-size: medium;"> </span></span>
<p><span style="font-family: comic sans ms,sans-serif;"><span style="font-size: medium;"><strong>&nbsp;Psycho Number</strong></span></span><strong> </strong></p>
<p><strong>&nbsp;</strong></p>
</td>
</tr>
</tbody>
</table>
<pre><span style="font-family: comic sans ms,sans-serif;"><span style="font-size: medium;"><span style="white-space: normal;"><pre><span style="white-space: normal;"><p>&nbsp;</p>
<pre><span style="font-family: arial,helvetica,sans-serif;"><span style="font-size: small;"><span style="text-decoration: underline;">Note</span> : 0 and 1 is not a psycho number .<br><span style="font-family: comic sans ms,sans-serif;">Psycho 1 : <strong><a title="Psycho Number" href="../PSYCHON/" target="_blank">Psycho</a></strong><br>Psycho 3 : </span></span></span><span style="font-family: comic sans ms,sans-serif;"><span style="font-size: small;"><span style="white-space: normal;"><strong><a href="../PSYCHO3/" target="_blank">Make Psycho</a>&nbsp;</strong></span></span></span></pre>
<pre><span style="white-space: normal; font-family: arial, helvetica, sans-serif;"><span style="font-size: small;"><span style="font-family: 'comic sans ms', sans-serif;">Psycho 4 :&nbsp;<span style="text-decoration: underline;"><a title="Psycho34 (easy)" href="../PSYCHOT" target="_blank"><strong>Psycho34 (easy)</strong></a></span></span></span></span><span style="font-weight: bold; white-space: normal; font-family: 'comic sans ms', sans-serif;"><span style="font-size: small;"><strong>&nbsp;</strong></span></span></pre>
<pre><span style="font-family: arial,helvetica,sans-serif;"><span style="font-size: small;">&nbsp;<br></span></span></pre>
</span></pre>
<hr>
<span style="font-size: small;"><strong><span style="text-decoration: underline;">Problem setter</span>:&nbsp;&nbsp; Shipu Ahamed, Dept. of CSE</strong></span></span></span></span><span style="font-size: small;"><strong><em><br><span style="font-family: arial,helvetica,sans-serif;">Bangladesh University of Business and Technology (BUBT)</span></em></strong></span><span style="font-family: arial,helvetica,sans-serif;"><span style="font-size: small;"><span style="white-space: normal;">&nbsp;</span></span></span></pre>
</span></pre>