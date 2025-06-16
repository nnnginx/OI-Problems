<p>Everyone knows that how much Shahjahan loved Mumtaaz, that he got built the Taj Mahal in the memory of his beloved Mumtaaz. Once Mumtaaz had fight with Shahjahan and she went to her father's home. Shahjahan then wrote a letter to Mumtaaz requesting her to come back, but then suddenly he realized that it is not safe to write letter in plain format (non-encoded message), so he thought whole day for a good method of encryption and then came up with a great idea of decoding his messages.<br><br>The technique of encoding messages used by Shahejahan is describes as-<br>1. A <b>key K</b> is set of digits (0-9) such that its value doesn't exceed <b>10<sup>6</sup></b>.<br>2. A <b>message M</b> is set of small letters (a-z) such that its length doesn't exceed <b>500</b>.<br>3. The <b>encoding function F(m, k) = m'</b> is a function that takes one digit from key and one character from message and encode it to another character.<br><br>The encoding algorithm is given by following pseudo code-
<br><br><font color="red">start of code</font>
</p><ol>
1. Repeat until message has characters to be encoded.<br>
<ol>
2. Read next <b>character c</b>, of message.<br>
3. Read next <b>digit k</b>, of key.<br>
4. Encode using the <b>function F(m, k) = m' : m' = m + k</b>.<br>
<ol>
5. If last digit k, of key is read then start reading in reverse order.<br>
6. If first digit k, of key is read while reading in reverse order, then start again reading in forward direction.<br>
</ol>
</ol>
</ol>
<p><font color="red">end of code</font></p>
<p><b>The addition operation to characters is cyclic</b>. Consider the following examples demonstrating the operator-<br>
1. 'a' + 2 = 'c'<br>
2. 't' + 1 = 'u'<br>
3. 'z' + 2 = 'b'<br>
4. 'y' + 0 = 'y'<br><br>
Consider the following encoding of message <b>"mumtaaz"</b> with key <b>132</b>-<br>
</p>
<table border="1" width="250" align="center">
<tbody><tr><th>Character c</th>
<th>Digit k</th>
<th>F(c, k)</th>
</tr><tr><td align="center">m</td><td align="center">1</td><td align="center">n</td></tr>
<tr><td align="center">u</td><td align="center">3</td><td align="center">x</td></tr>
<tr><td align="center">m</td><td align="center">2</td><td align="center">o</td></tr>
<tr><td align="center">t</td><td align="center">2</td><td align="center">v</td></tr>
<tr><td align="center">a</td><td align="center">3</td><td align="center">d</td></tr>
<tr><td align="center">a</td><td align="center">1</td><td align="center">b</td></tr>
<tr><td align="center">z</td><td align="center">1</td><td align="center">a</td></tr>
</tbody></table>
<br>
<p>So message "mumtaaz" is encoded as <b>"nxovdba"</b></p><br>.
<h3>Input</h3>
<p>First line of input it <b>T</b> (T &lt; 10001), total number of test cases.<br>
Each test case is consist of two lines, the first line contains key and second line contains encoded message.

</p><h3>Output</h3>
<p>For each test cases, output the original message in single line. 

</p><h3>Example</h3>

<pre><b>Input:</b>
6
132
nxovdba
212
uitktjvjmc
011
lfbejngafspsasfjnposubot
123
jnrygzpw
11
lfbejngafspsasfjnposubot
130
behipbobu<br>

<b>Output:</b>
mumtaaz
shrishtika
leadingzerosareimportant
iloveyou
keadimfzerorzreimonrtans
abhimanyu
</pre>