<p>Strings represented in computers often include special characters which are not printed, instead they have some other function, such as the newline character '\n'.</p>
<p>For ease of manipulation, these characters are usually represented by a regular character, preceded by a so called 'escape' - in the above example, the character '\'.</p>
<p>Buj recently bought a string <strong>S</strong> of length <strong>n</strong> on the local market, for (according to him completely legal and within the law) home manipulation.</p>
<p>He forgot to read the online store ratings and customer reviews.</p>
<p>Upong arriving at home and taking the string out of the unbelievably eco-unfriendly packaging, he realized with horror that the characters of the string do not follow any known encoding. The only thing he managed to do was number the characters from <strong>0 </strong>to <strong>n-1</strong> in perceived lexicographical order.</p>
<p>Oh well, thought Buj, I'll still manipulate this string to my heart's content... but what if I got scammed, and sold a low-quality string? One which, if it was printed out, would be lexicographically large?</p>
<p>But what would be printed out depends on which character in the string is the escape.</p>
<p>Buj sent us the string by post for analysis, and we uploaded it to this website hoping someone would do the work for us.</p>
<h3>Input</h3>
<p>The first line contains an integer <strong>1 ¡Ü T ¡Ü 10</strong> - the number of test cases. <strong>T</strong> cases follow.</p>
<p>For each case, the first line contains the number<strong><strong> </strong>n</strong> - the length of the string - and the second line contains a space-separated permutation of the numbers <strong>0, ... , n-1</strong> - the characters of the string.</p>
<p>The sum of <strong>n</strong> within an input file will not exceed <strong>10<sup>6</sup></strong>.</p>
<h3>Output</h3>
<p>In this problem, escape characters work as follows: if it is the last character in the string, it has no effect and is simply printed out as usual. Otherwise, that character and the character immediately following it is not printed (and instead together they have some other, printing-unrelated function). Take a look at the sample for clarification.</p>
<p>Let <strong>s<sub>i</sub></strong> be the string which would be printed if we choose character number <strong>i </strong>as the escape character.</p>
<p>Let <strong>p</strong><sub><strong>i</strong></sub> be the 0-based position of <strong>s<sub>i </sub></strong>if we sort all such strings lexicographically.</p>
<p>Output in a single line the numbers <strong>p<sub>0</sub></strong>, <strong>p<sub>1</sub></strong>, ..., <strong>p<sub>n-1</sub></strong>.</p>
<p>In other words, output in order the answer to the questions</p>
<p>"How many strings out of <strong>s<sub>0</sub></strong>, ..., <strong>s<sub>n-1</sub></strong> are lexicographically smaller than <strong>s<sub>0</sub></strong>?"</p>
<p>"How many are smaller than <strong>s<sub>1</sub></strong>?"</p>
<p>...</p>
<p>"How many are smaller than <strong>s<sub>n-1</sub></strong>?"</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>3<br>0 1 2<br>3<br>0 2 1<br><strong>Output:</strong>
2 0 1<br>2 1 0</pre>
<p>In the first case:</p>
<p>If character 0 was the escape, the printed string would be 2.</p>
<p>If 1 was the escape, the printed string would be 0.</p>
<p>If 2 was the escape, the printed string would be 0 1 2.</p>
<p>Ordering these strings, we get [0, 0 1 2, 2].</p>
<p>So <strong>s<sub>0</sub></strong> is at index 2, <strong>s</strong><sub><strong>1</strong> </sub>at index 0, and <strong>s<sub>2</sub></strong> at index 1, so the output is 2 0 1.</p>
<p>Note that the <strong>i</strong>-th number in the output is for the string where character <strong>number i</strong> is the escape, not the <strong>i</strong>-th character in the input.</p>