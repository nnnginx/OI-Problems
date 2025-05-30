<p align="justify">
In one of the internet banks thousands of operations are being performed every day. Since certain customers do business more actively than others, some of the bank accounts occur many times in the list of operations. Your task is to sort the bank account numbers in ascending order. If an account appears twice or more in the list, write the number of repetitions just after the account number.
The format of accounts is as follows: <b>2</b> control digits, an <b>8</b>-digit code of the bank, <b>16</b> digits identifying the owner (written in groups of four digits), for example (at the end of each line there is exactly one space):
</p><table align="center"><tbody><tr><td bgcolor="navy"><font color="yellow"><b>30 10103538 2222 1233 6160 0142&nbsp;</b></font></td></tr></tbody></table><p></p>
<p>
<b>Banks are real-time institutions and they need FAST solutions. If you feel you can meet the challenge within a very stringent time limit, go ahead!</b> A well designed sorting algorithm in a fast language is likely to succeed. </p><h3>Input</h3>
<p align="justify">
<br><i>t</i> [the number of tests &lt;= <b>5</b>]
<br><i>n</i> [the number of accounts&lt;= <b>100 000</b>]
<br>[list of accounts]
<br>[empty line]
<br>[next test cases]
</p>
<h3>Output</h3>
<p align="justify">
<br>[sorted list of accounts with the number of repeated accounts]
<br>[empty line]
<br>[other results]
</p>
<h3>Example</h3>
<pre><b>Input:</b>
2
6
03 10103538 2222 1233 6160 0142 
03 10103538 2222 1233 6160 0141 
30 10103538 2222 1233 6160 0141 
30 10103538 2222 1233 6160 0142 
30 10103538 2222 1233 6160 0141 
30 10103538 2222 1233 6160 0142 

5
30 10103538 2222 1233 6160 0144 
30 10103538 2222 1233 6160 0142 
30 10103538 2222 1233 6160 0145 
30 10103538 2222 1233 6160 0146 
30 10103538 2222 1233 6160 0143 

<b>Output:</b>
03 10103538 2222 1233 6160 0141 1
03 10103538 2222 1233 6160 0142 1
30 10103538 2222 1233 6160 0141 2
30 10103538 2222 1233 6160 0142 2

30 10103538 2222 1233 6160 0142 1
30 10103538 2222 1233 6160 0143 1
30 10103538 2222 1233 6160 0144 1
30 10103538 2222 1233 6160 0145 1
30 10103538 2222 1233 6160 0146 1
</pre>