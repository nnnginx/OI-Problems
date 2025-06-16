<p>Krishna loves Radha and wants to propose her in a different way. He wants to tell her the message, but he wanted the message to be a surprise. So, he plans to encrypt the message and send the encrypted message to Radha and he also gives the key to decrypt. He thinks that this might be a surprise to Radha. Help Radha to decrypt the message.</p>
<p><span style="text-decoration: underline;"><strong>Rules of encryption</strong></span> :</p>
<p>0&lt;=key&lt;=51</p>
<p>The original message only consists of a-z, A-Z, and space.</p>
<p>Spaces are encrypted as '.'</p>
<p>If key lies between 0 and 25, then the character is added with the key and modulo is taken and the case is maintained. For eg, if key is 3, then a is decrypted to d and e is decrypted to h.</p>
<p>If key lies between 26 and 51, then the character is added with the key and modulo is taken and the case is inverted. For eg, if key is 29, then a is decrypted to D and E is decrypted to h.</p>
<h3>Input</h3>
<p>First line consists of t, the number of test cases. (1&lt;=t&lt;=20)</p>
<p>For each test case, first line consists of key. 0&lt;=key&lt;=51</p>
<p>Second line consists of the encrypted message S. |S| &lt;= 100000</p>
<h3>Output</h3>
<p>For each test case, display the decrypted message in a separate line.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1<br>2<br>dsz.dsf<br><strong>Output:</strong>
fub fuh
</pre>