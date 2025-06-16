<p style="font-family: 'Times New Roman'; font-size: medium;">Encrypting passwords is one of the most important problems nowadays, and you trust only the encryption algorithms which you invented, and you have just made a new encryption algorithm.</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">Given a password which consists of only lower case English letters, your algorithm encrypts this password using the following 3 steps (in this given order):</p>
<ol style="font-family: 'Times New Roman'; font-size: medium;">
<li>Swap two different characters of the given password (you can do this step zero or more times).</li>
<li>Append zero or more lower case English letters at the beginning of the output of step one.</li>
<li>Append zero or more lower case English letters to the end of the output of step two.</li>
</ol>
<p style="font-family: 'Times New Roman'; font-size: medium;">And the encrypted password is the output of step three.</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">You have just finished implementing the above algorithm and applied it on many passwords. Now you want to make sure that there are no bugs in your implementation, so you decided to write another program which validates the output of the encryption program. Given the encrypted password and the original password, your job is to check whether the encrypted password may be the result of applying your algorithm on the original password or not.</p>
<p><span style="font-size: 1.17em;">Input</span></p>
<p><span style="font-family: 'Times New Roman'; font-size: medium;">Your program will be tested on one or more test cases. The first line of the input will be a single integer&nbsp;</span><span style="font-family: 'Times New Roman'; font-size: medium;"><em>T</em></span><span style="font-family: 'Times New Roman'; font-size: medium;">, the number of test cases&nbsp;</span><span style="font-family: 'Times New Roman'; font-size: medium;">(1<img src="file://9hAaW1Pq.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE"><em>T</em><img src="file://wXbQuPzf.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE">100)</span><span style="font-family: 'Times New Roman'; font-size: medium;">. Followed by the test cases, each test case is on two lines. The first line of each test case contains the encrypted password. The second line of each test case contains the original password. Both the encrypted password and the original password are at least 1 and at most 100,000 lower case English letters (from `</span><tt>a</tt><span style="font-family: 'Times New Roman'; font-size: medium;">' to `</span><tt>z</tt><span style="font-family: 'Times New Roman'; font-size: medium;">'), and the length of the original password is less than or equal the length of the encrypted password.</span></p>
<h3>Output</h3>
<p><span style="font-family: 'Times New Roman'; font-size: medium;">For each test case, print on a single line one word, `</span><tt>YES</tt><span style="font-family: 'Times New Roman'; font-size: medium;">' (without the quotes) if applying the algorithm on the original password may generate the encrypted password, otherwise print `</span><tt>NO</tt><span style="font-family: 'Times New Roman'; font-size: medium;">' (without the quotes).</span></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<pre>3</pre>
<pre>abcdef</pre>
<pre>ecd</pre>
<pre>cde</pre>
<pre>ecd</pre>
<pre>abcdef</pre>
<pre>fcd</pre>
<strong>Output:</strong>
<pre>YES
YES
NO</pre>
<span style="white-space: normal;"> </span></pre>