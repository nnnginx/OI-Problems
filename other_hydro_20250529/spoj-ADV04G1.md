<p>Regular expression is an expression which defines a set of strings. In this problem regular expression will contain only small latin letters a-z and special characters ¡®?¡¯, ¡®*¡¯ §Ú ¡®+¡¯. Each letter corresponds to itself in the defined strings. Special character can occur only after some letter and means the number of repetitions of the letter:</p>
<div align="center">
<table border="1" cellspacing="0" cellpadding="1"><tbody><tr><td align="left" nowrap=""> Character</td><td align="left" nowrap="">Repetitions</td></tr>
<tr><td align="left" nowrap=""> <tt>?</tt></td><td align="left" nowrap="">none or one</td></tr>
<tr><td align="left" nowrap=""> <tt>*</tt></td><td align="left" nowrap="">none or more</td></tr>
<tr><td align="left" nowrap=""> <tt>+</tt></td><td align="left" nowrap="">one or more</td></tr>
</tbody></table>
</div>
<p>For example ¡°ac¡±, ¡°abc¡±, ¡°acc¡±, ¡°abcccc¡±, and so on match regular expression ¡°ab?c+¡±.

For the given string find the substring which matches the given regular expression. If there are many such substrings find the most left one. If there are many of those as well fing the longest one.

</p><h3>Input</h3>
<p>The first line of input contains number T - the amount of test cases. The description of T test cases follows. The first line of each test case is the given string S of length L. Next line contains number n - the amount of regular expressions. Next n lines describe one regular expression Ri each for which you should find the matching substrings.

</p><h3>Constraints</h3>
<p>1 &lt;= T &lt;= 100<br>
1 &lt;= n &lt;= 10<br>
1 &lt;= L &lt;= 200<br>
1 &lt;= R<sub>i</sub> &lt;= 100

</p><h3>Output</h3>
<p>For each regular expression print the matching substring or -1 if there is no such substring in the given string.

</p><h3>Example</h3>

<pre><b>Input:</b>
1
aabbcc
5
b*c
a?b+c+
ab?c
b?c?
a?b?c?

<b>Output:</b>
bbc
abbcc
-1

a

</pre>