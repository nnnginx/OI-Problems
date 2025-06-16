<p><img src="./25041/file/nrSxcvIb.png" style="float:left">Yoda is the wisest, and perhaps the most powerful Jedi of his time. Yoda is a mysterious figure and he has many oddities. One of them is that Yoda often changes the order of words in the sentence. For example, one of such phrases is "Or I will help you not." Let's call the yodaness level of any statement the number of pairs of words that changed their order, as to the order in which they were supposed to go in a normal statement. Write a program that determines the yodaness level of different statement of Yoda.
</p><div style="clear:both">&nbsp;</div>

<h3>Input</h3>
<p>The first line of input contains the number t - the number of tests. Next comes the description of t tests. Each test consists of three rows. The first line of the test contains an integer n - number of words in the statement. The next line contains n words separated by spaces - the statement as Yoda says it. The next line is n words separated by spaces - the same statement as it should be said normally. All the words in the statement are different and consist of small latin letters.

</p><h3>Constraints</h3>
<p>1 &lt;= t &lt;= 10<br>
1 &lt;= n &lt;= 30000<br>
the length of each word does not exceed 20 characters


</p><h3>Output</h3>
<p>For each test print the yodaness level of the statement.

</p><h3>Example</h3>

<pre><b>Input:</b>
2
6
in the force strong you are
you are strong in the force
6
or i will help you not
or i will not help you

<b>Output:</b>
11
2

</pre>