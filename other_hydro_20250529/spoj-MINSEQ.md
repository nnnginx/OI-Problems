<p>Given two strings A and B, your are to find the lexicographically smallest string after inserting B into A.</p>
<p>For example, string A is "369", and string B is "4799". There are 4 ways that I can insert B into A, and I¡¯ll get 4 different results: 4799369, 3479969, 3647999, 3694799. Thus, 3479969 is the lexicographically smallest one.</p>
<h3>Input</h3>
<p>Input contains several cases. Each case has 2 strings A and B with length no longer than 100000 in 2 lines. Process the input until EOF. The strings consist of only digit 1-9.</p>
<h3>Output</h3>
<p>For each case, output the minimal possible result.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>369<br>4799<br>666<br>12345<br><br><strong>Output:</strong><br>3479969<br>12345666</pre>