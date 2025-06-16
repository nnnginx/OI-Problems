<p>
With water from the stream Galadriel filled the basin to the brim, and breathed on it, and when the water was still again she spoke. 'Here is the Mirror of Galadriel,' she said. 'I have brought you here so that you may look in it, if you will. For this is what your folk would call magic, I believe; though I do not understand clearly what they mean; and they seem also to use the same word of the deceits of the Enemy. But this, if you will, is the magic of Galadriel. Did you not say that you wished to see Elf-magic?' - Galadriel to Frodo and Sam, describing her Mirror.
</p>
<p>
We call a string S magical if every substring of S appears in Galadriel's Mirror (under lateral inversion). In other words, a magical string is a string where every substring has its reverse in the string.
</p>
<p>
Given a string S, determine if it is magical or not.
</p>

<h3>Input</h3>
<p>The first line contains T, the number of test cases. The next T lines contain a string each.&nbsp;</p>

<h3>Output</h3>
<p>For each test case, output "<tt>YES</tt>" if the string is magical, and "<tt>NO</tt>" otherwise.</p>

<h3>Constraints</h3>
<p>
1 &lt;= T &lt;= 100<br>
1 &lt;= |S| &lt;= 10<br>
S contains only lower-case characters.
</p>

<h3>Example</h3>
<pre><strong>Sample Input:</strong>
2
aba
ab

<strong>Sample Output:</strong>
YES
NO</pre>

<h3>Notes / Explanation of Sample Input</h3>
<p>For the first test case, the list of substrings are : a, b, ab, ba, aba. The reverse of each of these strings is present as a substring of S too.</p>
<p>For the second test case, the list of substring are : a, b, ab. The reverse of "ab", which is "ba" is not present as a substring of the string.</p>