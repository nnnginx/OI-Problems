<div align="justify">
<p>
Mathews uses a brand new 16-bit instruction processor. (Yeah i am being sarcastic!). It has one register (say R) and it supports two instructions: <br>
</p><ul>
<li>ADD X; Impact: R = (R + X) mod 65536
</li><li>MUL X; Impact: R = (R * X) mod 65536
</li><li>[For both instructions 0 &lt;= X &lt;= 65535]
</li></ul>
Mathews sees a segment of code, but doesnot know what value the register had before the code was being executed. How many possible values can the register have after the segment completed execution?
<p></p>
<br>
<b>Input Format:</b><br>
The input file consists of multiple testcases. <br>
The first line of each testcase contains one integer, <b>N</b>. (1 &lt;= N &lt;= 100,000).<br>
The following <b>N</b> lines contain one instructions each. <br>
Input terminates with a line containing N=0, which must not be processed. <br>
<br>
<b>Output Format:</b><br>
For each testcase print one integer in a single line, denoting the number of different values the register can take after code execution.<br>
<br>
<b>Sample Input:</b><br>
<pre>1
ADD 3
1
MUL 0
5
MUL 3
ADD 4
MUL 5
ADD 3
MUL 2
8
ADD 32
MUL 5312
ADD 7
MUL 7
ADD 32
MUL 5312
ADD 7
MUL 7
0
</pre>

<b>Sample Output:</b><br>
<pre>65536
1
32768
16
</pre>
</div>