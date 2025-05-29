<p>Sanky is a school kid and is very fond of numbers. His teacher gave his class a home work, asking each of them to invent a new series of numbers, with a large collection of numbers in them. His friend Evan has already invented one, which starts from 0 and picks every alternate number : {0, 2, 4 ,...} and he named them 'Evan' numbers :). Sanky is not happy because he couldn't invent that first and thinks picking every alternate number starting from 1 : {1, 3, 5, ... } would not be very odd ;).</p>
<table border="0">
<tbody>
<tr>
<td>
<p align="justify">After refreshing at home, he comes up with a new series of numbers in which the digits alternate between increasing and decreasing when compared with the digit before it, in a zig-zag fashion. To make it clear, if the number is abcde, either a &lt; b &gt; c &lt; d &gt; e or a &gt; b &lt; c &gt; d &lt; e. He cleverly named them 'Snaky Numbers' :). Eg: 8, 90, 243516 and 31524 are Snaky while 44, 123 and 4235 are not. He is now wondering if his Snaky series is large enough. Particularly, he wants to know how many 'Snaky Numbers' are there of length <em>at most</em> <strong>N</strong>. Count only non-negative integers, without leading zeros.</p>
</td>
<td>
<p><img src="./24376/file/yxyAXVYE.png" border="0" alt="" width="146" height="103"></p>
</td>
</tr>
</tbody>
</table>
<p>The answer may get very big and not fit in Sanky's book, so please just tell him the ( answer modulo <strong>M</strong> )</p>
<h3>Input</h3>
<p>First line contains T [ number of test cases, around 50 ].  Each of the next T lines contains two integers N M.</p>
<p>1 &lt;= N &lt;= 1,000,000,000</p>
<p>2 &lt;= M &lt;= 1,000,000,007</p>
<h3>Output</h3>
<p>For each test case, output  ( Number of Snaky numbers of length at most N ) % M, in a separate line</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>3<br>1 101<br>2 107<br>3 1001<br><br><strong>Output:</strong><br>10<br>91<br>616<br><br></pre>
<p><strong><span style="text-decoration: underline;"><em>&nbsp;Hint:</em></span></strong> You may have to use the mod operator wisely !</p>
<p><br> <em>* There are multiple test sets, and the judge shows the <strong>sum</strong> of the time taken over all test sets of your submission, if Accepted.</em></p>