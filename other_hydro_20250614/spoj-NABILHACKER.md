<p>
</p><p><strong style="font-weight: bold;">Credit:</strong></p>
<p><strong style="font-weight: bold;">Problem Set and Data set: Yasir Uddin Ahamed (Nabil)</strong></p>
<p><strong style="font-weight: bold;">Alternet Solution: Iqbal Hossain Bappy</strong></p>
<p></p>
<p>Many people asked me what actually contest programming do in real life projects. That does not feel&nbsp;so interesting to me. What I found interesting is, one day a hacker friend came to me. He asked me to solve one of his hacking problems.</p>
<p>When you try to steal someone's password, you may set a keylogger in his/her computer. Keylogger will give you a string that is typed as the password. But there is a problem, it will give you everything victim typed such as&nbsp;left key, right key, backspace everything. (Left key and right key means the keys you use to play car games, and backspace is the key you use to remove a letter, the button on the top of "Enter"&nbsp;button. )</p>
<p>Suppose, the victim typed "generio312" as password, but he follows these criteria:</p>
<p>1. he typed generio1.</p>
<p>2. Then he pressed the left key, and press 3. So the password will be generio31.</p>
<p>3. Then he pressed the right key and press 2. So the password will be generio312.</p>
<p>4. Now he typed&nbsp;ghj&nbsp;and then press backspace&nbsp;three times and remove these three letters. So the final password is generio312.</p>
<p>But, as I said, keylogger gives you all the typed key. You will get "generio1&lt;3&gt;2ghj---". (Here, &lt; for&nbsp;left&nbsp;key, &gt; for right key and - for backspace.)</p>
<h3>Input</h3>
<p><span style="font-size: 7.5pt; line-height: 107%; font-family: Verdana, sans-serif;">At first input T, the number of test cases.<br>Then input T strings. 1&lt;=|s|&lt;=10^6. The strings will include upper case, lower case, &lt;, &gt;, - and digits(0-9).</span></p>
<h3>Output</h3>
<p>The output&nbsp;should contain a string each line, the password.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p>2</p><p>&lt;&lt;BP&lt;A&gt;&gt;Cd-</p><p>ThisIsS3Cr3t</p><strong>Output:</strong>
<p>BAPC</p><p>ThisIsS3Cr3t </p><p>&nbsp;</p></pre>