<p><span style="font-size: small;"><br></span></p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;"><span style="font-size: small;">Problem Statement :</span></span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;"><span style="font-size: small;">You are given millions of words from a book.</span></span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;"><span style="font-size: small;">For each query you are given a string S. Find the most occuring word in the book with S as prefix.</span></span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;"><span style="font-size: small;">Input :</span></span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;"><span style="font-size: small;">The first line consists of an integer n, the number of words in the text book. The next n lines consists of the words in the book. The next line consists of an integer q, the number of queries. Next q lines consists a string S.</span></span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;"><span style="font-size: small;">Output:</span></span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;"><span style="font-size: small;">For each query String S, print the most occuring word in the book with S as prefix. If there are many such words, print the lexicographically smallest word. If there is no such word, print -1.</span></span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;"><span style="font-size: small;">Input Constraints :</span></span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;"><span style="font-size: small;">1 &lt;= n &lt;= 2*10^6</span></span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;"><span style="font-size: small;">1 &lt;= q &lt;= 10^6</span></span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;"><span style="font-size: small;">1 &lt;= word length &lt;= 10</span></span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;"><span style="font-size: small;">All the characters in the word are small letters of English alphabet.</span></span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;"><span style="font-size: small;">Example :&nbsp;</span></span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;"><span style="font-size: small;">Sample Input :</span></span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;"><span style="font-size: small;">5</span></span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;"><span style="font-size: small;">pen</span></span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;"><span style="font-size: small;">pine</span></span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;"><span style="font-size: small;">apple</span></span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;"><span style="font-size: small;">apple</span></span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;"><span style="font-size: small;">pen</span></span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;"><span style="font-size: small;">3</span></span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;"><span style="font-size: small;">p</span></span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;"><span style="font-size: small;">apple</span></span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;"><span style="font-size: small;">pi</span></span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;"><span style="font-size: small;">Sample Output :</span></span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;"><span style="font-size: small;">pen</span></span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;"><span style="font-size: small;">apple</span></span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;"><span style="font-size: small;">pine</span></span></div>
<p><span style="font-size: small;"><strong><span style="font-size: small;">Problem Statement :<br>&nbsp;</span></strong></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">You are given hundreds of thousands of words from a book.</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">For each query you are given a string S. Find the most occuring word in the book with S as prefix.</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;"><br></span></span></p>
<p><span style="font-size: small;"><strong><span style="font-size: small;">Input :<br>&nbsp;</span></strong></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">The first line consists of an integer n, the number of words in the text book. The next n lines consists of the words in the book. The next line consists of an integer q, the number of queries. Next q lines consists a string S.</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;"><br></span></span></p>
<p><span style="font-size: small;"><strong><span style="font-size: small;">Output:<br>&nbsp;</span></strong></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">For each query String S, print the most occuring word in the book with S as prefix along with the number of occurances of that word.<strong> If there are many such words, print the lexicographically smallest word. If there is no such word, print -1.</strong></span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;"><br></span></span></p>
<p><span style="font-size: small;"><strong><span style="font-size: small;">Input Constraints :</span></strong></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">1 &lt;= n &lt;= 5*10^5</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">1 &lt;= q &lt;= 10^5</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">1 &lt;= word length &lt;= 10</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">All the characters in the word are small letters of English alphabet.</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;"><br></span></span></p>
<p><span style="font-size: small;"><strong><span style="font-size: small;">Time Limit :</span></strong></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">3 seconds</span></span></p>
<p><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;"><strong><span style="font-size: small;">Sample Input :</span></strong></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">10</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">apple</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">banana</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">orange</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">applet</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">banana</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">oriental</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">orange</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">oriental</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">applet</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">bangalore</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">8</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">ban</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">bang</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">app</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">or</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">oriental</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">apple</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">hobbits</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">oranges</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;"><br></span></span></p>
<p><span style="font-size: small;"><strong><span style="font-size: small;">Sample Output :</span></strong></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">banana 2</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">bangalore 1</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">applet 2</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">orange 2</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">oriental 2</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">applet 2</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">-1</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">-1</span></span></p>
<p>&nbsp;</p>
<p><span style="font-size: small;"><span style="font-size: small;"><strong>Problem source</strong>: Inspired from autocomplete feature on google keyboard.</span></span></p>