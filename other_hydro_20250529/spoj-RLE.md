<p>Ram had to send large amount of data to his friend Vishnu. Since he was concerned about the time and the amount of data transfer it will take, he wanted to compress the data before he sent it. So he turns to you for help.</p>
<p>You need to perform run length encoding on a given string. The encoding is as follows : 'consecutive character count' followed by '!' followed by the 'character'. Do not encode the characters unless they lead to compression !</p>
<h3>Input</h3>
<p>Input consists of multiple lines of strings s, one string per line,&nbsp; with |s| &lt;= 100000 (read the input till EOF)</p>
<h3>Output</h3>
<p>For each input string, output a single line printing the run length encoding of the input string</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>aabbbbbccccc<br>aaaabbbbbbbbbbbbbbbccccc

<strong>Output:</strong>
aa5!b5!c<br>4!a15!b5!c
</pre>