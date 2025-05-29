<p>The city of <em><strong>Forum Boarium</strong></em> is full of temples . Unlike other cities the temples are built in a circular fashion in Forum Boarium &amp; each of these temples consists of exactly three floors. These floors are assigned a label,which is nothing but an<strong> </strong>English Alphabet.The speciality of the Circular arrangement of temples is that ,standing in any temple , we could see all other temples in the city . But over the years,all the temples have lost their sacredness except one .</p>
<p>Hercules arrives to this city, and wishes to visit the temple which is still sacred. An old wicked friend of Hercules leads him to the ground floor of the temple ,T1But knowing the nature of his wicked friend ,Hercules consults the old - aged people over there and finds the temple which still has its divine power ( T2 ). In order to reach T2 there are&nbsp; only two possible moves Hercules could do :</p>
<p>(i)Either shift between the floors of the same temple (or),</p>
<p>(ii)Jump between the same indexed floors( having same labels ) of two different temples . Some old ritual also says that, the labels of the corresponding floors other than the chosen one for jumping , must differ.</p>
<h3>Input</h3>
<p>The first line contains an integer t ( 1&lt;=t&lt;=10),the number of scenarios</p>
<p>t scenarios follow :</p>
<p>The first line of each scenario contains an integer N ( 2&lt;=N&lt;=3000), the number of temples. ( The temples are numbered from 1 to N ).</p>
<p>Each of the following N lines cotains the labels of the floors : a1,a2,a3 ( from bottom to top ).</p>
<p>The next line contains two integers :</p>
<p>T1 ( 1&lt;=T1&lt;=N ),the index of the temple he is currently in &amp; T2 ( 1&lt;= T2 &lt;=N),the index of the temple which is still divine.</p>
<h3>Output</h3>
<p>For each scenario print a single line - "Yes." , if the sacred temple could be reached , or otherwise "No.".</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1<br>3<br>a f r<br>a t p<br>x t m<br>1 3<br><br>&nbsp;<strong>Output:</strong>
Yes.
</pre>