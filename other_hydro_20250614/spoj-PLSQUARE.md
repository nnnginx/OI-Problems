<p>Kids just learnt about palindrome strings yesterday. Today, the teacher today was going to teach them about square shapes. &nbsp;But kids were still excited about palindrome strings. Therefore, the teacher came up with an idea combining square and palindrome in a game.</p>
<p>The teacher gave to kids a square board size of n, which is n row(s) * n column(s). Each row is a string of n character(s). Then, the teacher asked them to find the palindrome sub-square, which has maximum size. &nbsp;A palindrome sub-square is a sub square in board such that characters in each row of the sub square give out a palindrome string, and characters in each column of the sub square also give out a palindrome string.&nbsp;</p>
<p>Remember: A palindrome string is a string that has the property of reading the same in either direction, e.g. 'racecar', 'solos'.</p>
<p>When the teacher comes out from toilet, he was too happy and forgot the sub square in solution¡­ Your task now is to help him to find out the maximum size of the palindrome sub square in the given board.</p>
<p><strong>Input:</strong></p>
<p>The first row contains an integer n, which is the size of the board. n&lt;=200.</p>
<p>Each row in next n rows is a string contains only n lowercase characters, which describes the board.</p>
<p><strong>Output:</strong></p>
<p>Only 1 integer which is the maximum size of palindrome sub square in the board.</p>
<p><strong>Example:&nbsp;</strong></p>
<pre><strong><strong>Input 1:</strong></strong>
4</pre>
<pre>babb</pre>
<pre>acaz</pre>
<pre>babx</pre>
<pre>fdhk

<strong>Output 1:</strong>
3</pre>
<pre><strong>Input 2:</strong></pre>
<pre>1</pre>
<pre>a</pre>
<pre><strong>Output 2:</strong></pre>
<pre>1</pre>