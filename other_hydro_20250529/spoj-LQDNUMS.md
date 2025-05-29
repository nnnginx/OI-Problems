<p style="text-align: left;"><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;"> </span></p>
<p><span style="font-size: small;"> </span></p>
<p><span style="font-size: small;"> </span></p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">He choose a number N ( 1 ≤ N ≤ 10^18 ),&nbsp;</span></div>
<p><span style="font-size: small;"> </span></p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">then wrote all the numbers from 1 to N to form a continuous string of digits. Next he replaced substrings of indentical digits with a single digit. For example string fragment "14445556677666" would be changed to "145676". He named this shortened string S. Then he specified a problem for his fellow professors: given a length of string S determine the number N witch results in that kind of string S. The task has proven to be too much for Mathematicans. can you solve it?&nbsp;</span></div>
<p><span style="font-size: small;"> </span></p>
<p><span style="font-size: small;">During a meeting with professors in the Asian Confederation of Mathematics, a Russian professor came up with a problem:&nbsp;</span></p>
<p><span style="font-size: small;"> </span></p>
<p><span style="font-size: small;">He choose a number N ( 1 ≤ N ≤ 10^18 ),&nbsp;then wrote all the numbers from 1 to N to form a continuous string of digits. Next he replaced substrings of indentical digits with a single digit. For example string fragment "14445556677666" would be changed to "145676". Then he specified a problem for his fellow professors: given a length of string S determine the number N witch results in that kind of string S. The task has proven to be too much for Mathematicans. can you solve it?&nbsp;</span></p>
<p><span style="font-size: small;"> </span></p>
<p style="text-align: left;"><span style="font-size: small;"><strong>Your task: </strong></span></p>
<p><span style="font-size: small;"> </span></p>
<p style="text-align: left;"><span style="font-size: small;">Write a program to help your country's mathematicians.&nbsp;</span></p>
<p><span style="font-size: small;"> </span></p>
<h3 style="text-align: left;"><span style="font-size: small;">Input</span></h3>
<p><span style="font-size: small;"> </span></p>
<p style="text-align: left;"><span style="font-size: small;"><span title="Nhấp để xem bản dịch thay thế">A single number M, length of the string S&nbsp;&nbsp;( 1 ≤ M ≤ 10<sup>18&nbsp;</sup>)</span></span></p>
<p><span style="font-size: small;"> </span></p>
<h3 style="text-align: left;"><span style="font-size: small;">Output</span></h3>
<p><span style="font-size: small;"> </span></p>
<p style="text-align: left;"><span style="font-size: small;">A single number N, the number which Russian professor selected.&nbsp;</span></p>
<p><span style="font-size: small;"> </span></p>
<h3 style="text-align: left;"><span style="font-size: small;">Example</span></h3>
<p><strong>Input:</strong></p>
<pre>13</pre>
<p><strong>Output:</strong></p>
<pre>12</pre>
<p><strong>Explaination:</strong></p>
<pre>With N = 12, we get the string:
- 123456789101112
Because three consecutive number one in the same location adjacent to the end, we delete the first two numbers, then we have
- 1234567891012
The length of this string is 13</pre>