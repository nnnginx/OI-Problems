<p>
Your task is, given an integer N, to make a palindrome (word that reads the same when you reverse it) of length at least N (1 &lt;= N &lt;= 100,000). Any palindrome will do.</p>
<p>
Easy, isn't it? That's what you thought before you passed it on to your inexperienced team-mate. When the contest is almost over, you find out that that problem still isn't solved. The problem with the code is that the strings generated are often not palindromic. There's not enough time to start again from scratch or to debug his messy code.</p>
<p>
Seeing that the situation is desperate, you decide to simply write some additional code that takes the output and adds just enough extra characters to it to make it a palindrome and hope for the best. Your solution should take as its input a string and produce the smallest palindrome that can be formed by adding zero or more characters at its end. The input string will consist of  only upper and lower case letters.
</p>
<h3>Example</h3>

<pre><b>Input:</b>
aaaa
abba
amanaplanacanal
xyz

<b>Output:</b>
aaaa
abba
amanaplanacanalpanama
xyzyx
</pre>

<em>Note: 
<br>1. All palindromes are considered case-sensitive (i.e. 'Aa' is not a palindrome).
<br>2. Large I/O. Be careful in certain languages.
</em>