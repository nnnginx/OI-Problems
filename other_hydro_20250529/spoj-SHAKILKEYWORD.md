<p>Nahid bhai is a principal software engineer of a renowned software company. Rumman is an associate software engineer of that company. One day Nahid bhai assigned a task to Rumman. The task is to find all keywords from a given string. A keyword is a word that contains at least one ¡°#¡±. A word may contain other letters and punctuations. Given string will be split based on some delimiters. Rumman is so busy learning cutting edge technology for developing a project. So he assigned this task to you. You as a programmer will do the same thing.</p>
<p>For example: Given string is ¡°Here are some fruit name: #apple, #banana, #orange.¡±. Delimiters are ¡°|$ *@.&amp;\"!^,?¡±. So, the words containing ¡°#¡± will be: ¡°#apple¡±, ¡°#banana¡±, ¡°#orange¡±.</p>
<p><strong>Delimiters are, fixed for all string: ¡°|$ *@.&amp;\"!^,?¡±.</strong></p>
<h3>Input</h3>
<p>Input starts with the number of test cases, T (1&lt;=T&lt;=10).</p>
<p>Each line contains a string consisting letters and punctuations. (1&lt;=|string|&lt;=100).</p>
<h3>Output</h3>
<p>For each test case, print the keywords in a new line. If no keywords found, then print ¡°No keywords.¡±</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p>3</p><p>ab#c def#.</p><p>Abcde fghij</p>abc.efg#ijk #lMn.

<strong>Output:</strong>
<p>ab#c</p><p>def#</p><p>No keywords.</p><p>efg#ijk</p><p>#lMn</p></pre>