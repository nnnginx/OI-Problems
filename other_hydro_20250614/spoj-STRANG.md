<!-- pre.cjk { font-family: "Courier New",monospace; }p { margin-bottom: 0.1in; line-height: 120%; }code.cjk { font-family: "Courier New",monospace; } -->
<p style="margin-bottom: 0in; font-weight: normal; line-height: 100%;"><em>Someone thinks that someone thinks that someone thinks that...,<br></em></p>
<p style="margin-bottom: 0in; font-weight: normal; line-height: 100%;">Trang is a nice girl who is keen on learning English to make her study abroad dream come true. She practices everyday that her progress impresses the teacher. On Trang 's birthday, she receive an English book from her teacher. The interesting thing is that the book contain only one (very long) sentence ! Trang is surprised that she cannot understand any word and decides to learn every word in the sentence. She wants to learn the longest word first, but it should appear in the string a few times since Trang is curious about the meaning of the sentence. Help her to find the first word to learn !</p>
<p style="margin-bottom: 0in; font-weight: normal; line-height: 100%;">&nbsp;</p>
<p style="margin-bottom: 0in; font-weight: normal; line-height: 100%;">You are given a string S (the sentence), which its length can be up to 100000, including only lowercase alphabetical letters ('a'..'z'). A word is defined as a subtring of consecutive characters and each is assigned an ¡°important¡± value, which is equal ((length of the word) * (number of times it occurred in the sentence)).</p>
<p style="margin-bottom: 0in; font-weight: normal; line-height: 100%;">&nbsp;</p>
<p style="margin-bottom: 0in; font-weight: normal; line-height: 100%;"><strong>INPUT</strong>: One line containing the string S.</p>
<p style="margin-bottom: 0in; font-weight: normal; line-height: 100%;"><strong>OUTPUT</strong>: One number, the ¡°important¡± value of the most ¡°important¡± word.</p>
<p><span style="text-decoration: underline;"><em>Sample Input:</em></span></p>
<p>abcabcdddlo</p>
<p style="margin-bottom: 0in; font-weight: normal; line-height: 100%;">&nbsp;</p>
<p style="margin-bottom: 0in; font-weight: normal; line-height: 100%;"><span style="text-decoration: underline;"><em>Sample Output:</em></span></p>
<p style="margin-bottom: 0in; font-weight: normal; line-height: 100%;">11</p>
<p style="margin-bottom: 0in; font-weight: normal; line-height: 100%;"><span style="text-decoration: underline;"><br></span></p>
<p><span style="text-decoration: underline;"> </span></p>
<p style="margin-bottom: 0in; font-weight: normal; line-height: 100%;"><span style="text-decoration: underline;"><em>Sample Input:</em></span></p>
<pre style="font-weight: normal;"><code>aaaaaa</code></pre>
<p style="margin-bottom: 0in; font-weight: normal; line-height: 100%;">&nbsp;</p>
<p style="margin-bottom: 0in; font-weight: normal; line-height: 100%;"><span style="text-decoration: underline;"><em>Sample Output:</em></span></p>
<p style="margin-bottom: 0in; font-weight: normal; line-height: 100%;">12</p>