<p align="justify">
At the end of year 2004, the regional agencies of the Polish Military Recruitment Office (known as WKU in Polish) is sending a call to all boys born in 1984. Every recruit has his personal 11-digit identification number (PESEL, format: YYMMDDXXXXX, where YYMMDD is the date of birth, and XXXXX is a zero-padded integer smaller than 100000). Every agency of the Military Recruitment Office has its own code (MRO, format: a place code consisting of 3 upper case letters and a one-digit number). But this year the army underwent some reforms and not all boys at conscription age are going to be recruited. 
The list of closed down MRO points is as follows: the code of the closed down MRO is followed by the code of some other MRO, to which all the recruits are now going to be assigned. The list of recruits contains their PESEL codes. Your task is to prepare the complete list of 
recruits and determine the codes of their new MRO-s.
</p>
<h3>Input</h3>
<p align="justify">
</p><pre><i>s</i> [the number of tests &lt;= <b>10</b>]
<i>p</i> [the number of boys at conscription age &lt;= <b>100000</b>]
<i>PESEL and MRO code</i>
<i>z</i> [the number of closed down MRO points &lt;= <b>100000</b>]
<i>old_code new_code</i> [old_code - the code of closed down MRO,
new_code - its new MRO code]
<i>p</i> [the number of recruits &lt;= <b>100000</b>]
<i>PESEL</i> [PESEL code of recruit]
[empty line]
[next tests]
</pre>
<p></p>
<h3>Output</h3>
<p align="justify">
</p><pre>one PESEL and MRO code per line in the order of input
[empty line between tests]
[other results]
</pre>
<p></p>
<h3>Example</h3>
<pre>Input:
1
4
84101011111 GDA1
84010122222 GDA2
84010233333 GDA2
84020255555 GDY1
1
GDA2 GDA1
3
84101011111
84010122222
84020255555

Output:
84101011111 GDA1
84010122222 GDA1
84020255555 GDY1

</pre>
<b>Warning: large Input/Output data, be careful with certain languages</b>