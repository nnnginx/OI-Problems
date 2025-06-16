<p>
A string s is called an (k,l)-repeat if s is obtained by concatenating k&gt;=1 times some seed string t with length l&gt;=1. For example, the string 
</p><p>
s = abaabaabaaba
</p><p>
is a (4,3)-repeat with t = aba as its seed string. That is, the seed string t is 3 characters long, and the whole string s is obtained by repeating t 4 times. </p><p>
Write a program for the following task: Your program is given a long string u consisting of characters ¡®a¡¯ and/or ¡®b¡¯ as input. Your program must find some (k,l)-repeat that occurs as substring within u with k as large as possible. For example, the input string
</p><p>
u = babb<u>abaabaabaaba</u>b
</p><p>
contains the underlined (4,3)-repeat s starting at position 5. Since u contains no other contiguous substring with more than 4 repeats, your program must output the maximum k. 
</p><p>


</p><h3>Input</h3>
<p>
In the first line of the input contains H- the number of test cases (H &lt;= 20). H test cases follow. First line of each test cases is n - length of the input string (n &lt;= 50000), The next n lines contain the input string, one character (either ¡®a¡¯ or ¡®b¡¯) per line, in order. 
</p><h3>Output</h3>
<p>
For each test cases, you should write exactly one interger k in a line - the repeat count that is maximized. 
</p><h3>Example</h3>

<pre><b>Input:</b>
1
17
b
a
b
b
a
b
a
a
b
a
a
b
a
a
b
a
b

<b>Output:</b>
4
</pre>

since a (4, 3)-repeat is found starting at the 5th character of the input string.