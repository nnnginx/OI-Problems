<p><br>In the country of Thuvax lived an old wizard named Chanithpra. He practised a form of magic in which the power of spell came from the letters that were written on a piece of parchment. <br>When a sentence s is written, the intensity of the letters are as follows: <br>1. Intensity of 'a' is 1, 'b' is 2 and it continues till 'z' whose intensity is 26. <br>2. Intensity of 'A' is 51, 'B' is 52 and it continues till 'Z' whose intensity is 76. <br>3. Intensity of ' '(space) is 32. <br>&nbsp;<br>The power of a spell written as a part of the sentence is equal to the sum of the intensities of the characters present in it modulo m. <br>&nbsp;<br>Chanithpra finds an old parchment in Thuvax with a sentence s written on it. <br>Help him find the longest spell (i, i+1, ... j) in the sentence s whose power matches with k. (0&lt;=i&lt;=j&lt;length of s)<br>&nbsp;<br>You need to print the starting index i(0&lt;=i&lt;=length-1) of such a spell in the sentence and the length of the spell. &nbsp;<br>&nbsp;<br>If there are multiple such spells, find the minumum index i and if there is no such spell print -1.</p>
<h3>Input</h3>
<p>The first line contains a single positive integer t(1&lt;=t&lt;=100) denoting the number of test cases.<br>Each test case consists of 2 lines: <br>The first line consists of the sentence s(1&lt;=length of s&lt;=1000000). <br>The second line consists of two integers m and k (2&lt;=m&lt;=1000007 and 0&lt;=k&lt;m).</p>
<h3>Output</h3>
<p>For each test case, output one line containing 2 integers. The first is the minimum index i(0&lt;=i&lt;=s.length-1). The second is the length of the spell. <br>If no such spell is present, print -1</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1<br>Hello World<br>10 7

<strong>Output:</strong>
0 7
</pre>