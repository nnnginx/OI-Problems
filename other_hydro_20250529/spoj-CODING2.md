<p>A binary code for an alphabet of 2<strong><sup>N</sup></strong> symbols is a bijection between the 2<strong><sup>N</sup></strong> symbols and 2<strong><sup>N</sup></strong> binary codewords. For example, in the table below 3 different binary codes are presented for a 4-symbol alphabet (<strong>a</strong>,<strong>b</strong>,<strong>c</strong>,<strong>d</strong>).</p>
<table border="0" align="center">
<tbody>
<tr>
<th>Symbol </th><th>Code 1 </th><th>Code 2 </th><th>Code 3 </th>
</tr>
<tr>
<td>a</td>
<td>00</td>
<td>0</td>
<td>1</td>
</tr>
<tr>
<td>b</td>
<td>01</td>
<td>10</td>
<td>10</td>
</tr>
<tr>
<td>c</td>
<td>10</td>
<td>110</td>
<td>100</td>
</tr>
<tr>
<td>d</td>
<td>11</td>
<td>111</td>
<td>1000</td>
</tr>
</tbody>
</table>
<p>A code is said to be prefix-free if none of the codewords is a prefix of another codeword. For example, in the table above, codes 1 and 2 are prefix-free. However, code 3 is not prefix-free. Prefix-free codes are widely used, as encoding and decoding becomes very simple.<br>For this problem, given <strong>N</strong> and a message containing <strong>M</strong> alphabet symbols, the task is to find a prefix-free code for the entire alphabet (including symbols possibly not present in the message) that minimizes the number of necessary bits to represent the message. For example, let <strong>N</strong>=2, with symbols (a,b,c,d), and the message "<strong>a a a a b b b b a a a a c c d d</strong>"</p>
<p>The message encoded with codes 1 and 2 above becomes, respectively:</p>
<ul>
<li>00 00 00 00 01 01 01 01 00 00 00 00 10 10 11 11, for a total of 32 bits.</li>
<li>0 0 0 0 10 10 10 10 0 0 0 0 110 110 111 111, for a total of 28 bits.</li>
</ul>
<p>It is possible to show that no prefix-free code can encode the message above in less than 28 bits.</p>
<h3>Input</h3>
<p>The input contains several test cases. Each test case has two lines. The first line of a test case contains two integers <strong>N</strong>, <strong>M</strong> separated by a single space (1 �� <strong>N</strong> �� 15, 1 �� <strong>M</strong> �� 106, <strong>D</strong> �� 15).</p>
<p>On the second line are <strong>M</strong> integers <strong>X<sub>i</sub></strong>, 0 �� <strong>Xi</strong> �� 2<strong><sup>N</sup></strong> �C 1, representing the message to be encoded. The end of the input is marked by a case with <strong>N</strong>=<strong>M</strong>=0. This case must not be processed.</p>
<h3>Output</h3>
<p>For each test case, print a single line with one integer, the minimum number of bits necessary to encode the message using a prefix-free code.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2 16<br>0 0 0 0 1 1 1 1 0 0 0 0 2 2 3 3<br>0 0

<strong>Output:</strong>
28
</pre>