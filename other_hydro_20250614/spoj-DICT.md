<p>&nbsp;&nbsp;&nbsp; Eloy the byte is helping his son, Marcos the little one, with the homework, which consists on: Given one or more words you should search in the dictionary which word contains the proper prefix of the word given, for example<br>&nbsp;&nbsp; &nbsp;set is a prefix of setter, but also of setting.<br>&nbsp;&nbsp; &nbsp;Now, neither Eloy nor Marcos wants to search the words in the dictionary (they just won¡¯t do it)¡­ Marcos will give you the words in the dictionary and the words to find the prefix of¡­ You should make a program that given this, output the list of words that contains as a prefix the word given, Marcos can make mistakes sometimes, so, be careful! Marcos won¡¯t always be telling the real prefixes all the time, in addition, sometimes Marcos can repeat the same word (while reading the dictionary), in this case, the word should be treated as it was mentioned just <strong>one time</strong>.<br><br>&nbsp;&nbsp;&nbsp; <strong>INPUT</strong>:<br>&nbsp;&nbsp; &nbsp;The input will consist in an integer N (1&lt;=N&lt;=25.000), next, N lines will follow containing a single word (maximum of 20 characters (all lowercase letters)), after that, there will be an integer K (1&lt;=K&lt;=22.000) containing the number of words to look in the dictionary, then, K lines containing the prefix-word.<br><br>&nbsp;&nbsp;&nbsp; <strong>OUTPUT</strong>:<br>&nbsp;&nbsp;&nbsp; The output will consist in displaying the words that are composed from the word given, you should output ¡°Case #i:¡± where i is the i-th case, then, at the next line, output the list of the composed words (lexicographical-ordered), if there is none, you should output ¡°No match.¡±<br><br><strong>SAMPLE DATA:</strong></p>
<p><strong>INPUT:</strong></p>
<p>5</p>
<p>set</p>
<p>lol</p>
<p>setter</p>
<p>setting</p>
<p>settings</p>
<p>2</p>
<p>set</p>
<p>happy</p>
<p><strong>OUTPUT:</strong></p>
<p>Case #1:</p>
<p>setter</p>
<p>setting</p>
<p>settings</p>
<p>Case #2:</p>
<p>No match.</p>