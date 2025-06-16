<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/MBLAST/en/">English</a></td> 
<td width="50%"><a href="/problems/MBLAST/vn/">Vietnamese</a></td> 
</tr></tbody></table>

<p>
There are given two strings, A and B.  An expansion of some string X is a string created by adding or inserting any number (zero, one or more) of blanks anywhere in the string, or in the begining or the end of the string. Eg., if the string X is ¡®abcbcd¡¯, then the strings 'abcb-cd', '-a-bcbcd-' and 'abcb-cd-' are expansions of the string X (blanks are denoted by the character ¡®-¡®). </p>

<p>
If A1 is an expansion of the string A, and B1 is and expansion of the string B, and if A1 and B1 are of the same length, then we define the distance of the strings A1 and B1 as the sum of the distances of the characters on the same positions in these strings. We define the distance of two characters as the absolute difference of their ASCII codes, except the distance of the blank and another character, which is given (and equal for all characters). </p>

<p>
You are to write a program which finds the expansions A1 and B1 of strings A and B, that have the smallest difference. </p>
  
<h3>Input</h3>
<p>
The first line of the input file consists of the string A, and the second line of string B. They are consisted only of lower case characters of the english alphabet (a-z), and the number of characters in 
any of the strings is less than or equal to 2000.</p>
<p>
The third line consists of an integer K, 1 ¡Ü K ¡Ü 100, the distance of the blank and the other characters. </p>

<h3>Output</h3>
<p>The first only line of the input file should consist of the smallest distance as defined in the text of the task.</p>
 
<h3>Sample</h3><p>
</p><pre><b>Input:</b>
cmc
snmn
2

<b>output:</b>
10</pre>

<pre><b>Input:</b>
koiv
ua
1

<b>output:</b>
5</pre>

<pre><b>input:</b> 
mj
jao
4

<b>output:</b>
12</pre>