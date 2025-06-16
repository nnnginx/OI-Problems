<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/MREPLBRC/en/">English</a></td> 
<td width="50%"><a href="/problems/MREPLBRC/vn/">Vietnamese</a></td> 
</tr></tbody></table>

<p>
A regular bracket sequence is a string of characters consisting only of
opening and closing brackets, and satisfying the following conditions: </p><p>
•  An empty string is a regular bracket sequence. </p><p>
•  If A is a regular bracket0sequence, then (A), [A] and {A} are also 
regular bracket sequences. </p><p>
•  If A and B are regular bracket sequences, then AB is also a regular
bracket sequence. </p><p>
For  example,  the  sequences  [({})],  [](){}  i  [{}]()[{}]  
are  regular,  but  the  sequences  [({{([,  []({)}  and 
[{}])([{}] are not. </p><p>
Ivica has found a string which looks like it could be a regular bracket 
sequence. Some of the characters have become smudged and illegible, and 
could have been any character. </p><p>
Write a program that calculates how many ways the illegible characters
in the string can be replaced by brackets so that the result is a 
regular bracket sequence. This number can be very large, so output only 
its last 5 digits.</p><p>

</p><h3>Input</h3>
<p></p><p>
The first line contains an even integer N (2 &lt;= N &lt;= 200), the length of 
the string. </p><p>
The second line contains the string. Illegible characters are represented
by the '?' character. 
</p><p>
</p><h3>Output</h3>
<p></p><p>
Output the number of regular bracket sequences the string could have read. 
</p><p>
</p><h3>Sample</h3>
<pre>input 

6 
()()() 
 
output 
 
1 

input 
 
10 
(?([?)]?}? 
 
output 
 
3

input 
 
16 
???[???????]???? 
 
output 
 
92202

In  the  second example,  the  three matching  regular bracket sequences
are ({([()])}), ()([()]{}) and ([([])]{}).
</pre>