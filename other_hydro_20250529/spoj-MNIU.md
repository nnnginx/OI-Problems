<pre><span style="font-family: verdana, geneva;"><br></span><span style="white-space: normal;"><p><strong><span style="font-family: verdana, geneva;">My Name is UMMMM¡­.</span></strong></p>
<p><span style="font-family: verdana, geneva;">In a country far away there is a kind of a competition called programming contests. As they are becoming increasingly popular, they get regular coverage on newspapers. That's the only positive part of the story. The quality of their reports are not up to the mark and often hilarious for the competitive programming community. The reporters often mix up names - exchanging words from one person's name to someone else's name.</span></p>
<p><span style="font-family: verdana, geneva;">Chowdhury Shaheb - a curious programmer analyzed the reports and found a very interesting pattern. He saw whenever any word of two person's names have the same first and last letters and at least one additional common letter, journalists will mix them up. For example: The words ¡®Manjur¡¯ and ¡®Mazumder¡¯ have same first and last letters and two common letters 'a' and 'u'.</span></p>
<p><span style="font-family: verdana, geneva;">You'll be given a pair of names. List all possible confusing name variations of those two names. A confusing variation of a name is obtained by changing at least one word of that name to a similar word (according to the aforementioned pattern) from the other¡¯s name. A variation is <strong>not </strong>considered confusing if it is exactly same to any of the given names. See the input and output format section for more details.</span></p>
<p><strong><span style="font-family: verdana, geneva;">Input</span></strong></p>
<p><span style="font-family: verdana, geneva;">First line of input will contain a single integer T (1 &lt;= T &lt;= 15), the number of testcases. It will be followed by T sets of testcases. Each set of testcase will contain two lines, each line will contain a name. Each name will contain no more than 20 characters. Names will have no more than 3 words, each word will consist of only Engish letters (¡®A¡¯- ¡®Z¡¯ , ¡®a¡¯-¡®z¡¯). First letter of a word will always be capitalized and others are in lowercase. Each word of a name will be separated by exactly one space between them.</span></p>
<h4><span style="font-family: verdana, geneva;">Output</span></h4>
<p><span style="font-family: verdana, geneva;">First line of the output of each test case should contain the case number (In this format: Case &lt;casenumber&gt;:). From the next line, print all the confusing variations - one per line in ascending <strong>lexicographic order</strong>. A name X is lexicographically smaller than another name B if it contains a smaller letter at the first position they differ or if X is a prefix of Y. A space is smaller than any other English character. If there is no confusing name, print "None" (without the quotes). <strong>Print a blank line between testcases</strong>.</span></p>
<table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="319" valign="top">
<p><strong><span style="font-family: verdana, geneva;">Sample Input</span></strong></p>
</td>
<td width="319" valign="top">
<p><strong><span style="font-family: verdana, geneva;">Output for Sample Input</span></strong></p>
</td>
</tr>
<tr>
<td width="319" valign="top">
<p><span style="font-family: 'courier new', courier;">3</span></p>
<p><span style="font-family: 'courier new', courier;">Syed   Shahriar Manjur</span></p>
<p><span style="font-family: 'courier new', courier;">Pratyai   Mazumder</span></p>
<p><span style="font-family: 'courier new', courier;">Tasnim   Imran Sunny</span></p>
<p><span style="font-family: 'courier new', courier;">Sabbir   Yousuf Sanny</span></p>
<p><span style="font-family: 'courier new', courier;">Md   Hafiz Uddin</span></p>
<p><span style="font-family: 'courier new', courier;">Sohel   Hafiz</span></p>
</td>
<td width="319" valign="top">
<p><span style="font-family: 'courier new', courier;">Case   1:</span></p>
<p><span style="font-family: 'courier new', courier;">Pratyai   Manjur</span></p>
<p><span style="font-family: 'courier new', courier;">Syed   Shahriar Mazumder</span></p>
<p><span style="font-family: 'courier new', courier;"><br></span></p>
<p><span style="font-family: 'courier new', courier;">Case   2:</span></p>
<p><span style="font-family: 'courier new', courier;">Sabbir   Yousuf Sunny</span></p>
<p><span style="font-family: 'courier new', courier;">Tasnim   Imran Sanny</span></p>
<p><span style="font-family: 'courier new', courier;"><br></span></p>
<p><span style="font-family: 'courier new', courier;">Case   3:</span></p>
<p><span style="font-family: 'courier new', courier;">None</span></p>
</td>
</tr>
</tbody>
</table>
<p>Problem Setter: Mir Wasi Ahmed</p><p>Special Thanks: Ahmad Faiyaz</p></span></pre>