<p><span style="font-family: 'Times New Roman'; font-size: medium;">Consider the set of all non-negative integer powers of 3.</span></p>
<p><em>S</em>&nbsp;= { 1, 3, 9, 27, 81, ... }</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">Consider the sequence of all subsets of&nbsp;<em>S</em>&nbsp;ordered by the value of the sum of their elements. The question is simple: find the set at the&nbsp;<em>n</em>-th position in the sequence and print it in increasing order of its elements.</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">Each line of input contains a number&nbsp;<em>n</em>, which is a positive integer with no more than 19 digits. The last line of input contains 0 and it should not be processed.</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">For each line of input, output a single line displaying the&nbsp;<em>n</em>-th set as described above, in the format used in the sample output.</p>
<h3 style="font-family: 'Times New Roman';">Input</h3>
<pre>1
7
14
783
1125900981634049
0
</pre>
<h3 style="font-family: 'Times New Roman';">Output</h3>
<pre>{ }
{ 3, 9 }
{ 1, 9, 27 }
{ 3, 9, 27, 6561, 19683 }
{ 59049, 3486784401, 205891132094649, 717897987691852588770249 }</pre>