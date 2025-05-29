<p>Given two sequences of words: X=(x<sub>1</sub>,...,x<sub>n</sub>) and Y=(y<sub>1</sub>,...,y<sub>n</sub>), determine how many binary sequences P=(p<sub>1</sub>,...,p<sub>n</sub>) exist, such 
	that the word concatenation z<sub>1</sub>z<sub>2</sub>...z<sub>n</sub>, where z<sub>i</sub>=x<sub>i</sub> iff p<sub>i</sub>=1 and z<sub>i</sub>=y<sub>i</sub> iff p<sub>i</sub>=0,
	is a palindrome (a word which is the same when read from left to right and from 
	right to left).
</p>
<h3>Input</h3>
<p>
	The input begins with the integer t, the number of test cases. Then t test 
	cases follow.
</p>
<p>
	For each test case the first line contains the positive integer n - the number 
	of words in a sequence (1&lt;=n&lt;=30). The following n lines contain 
	consecutive words of the sequence X, one word per line. The next n lines 
	contain consecutive words of the sequence Y, one word per line. Words consist 
	of lower case letters of the alphabet ('a' to 'z'), are non-empty, and not 
	longer than 400 characters.
</p>
<h3>Output</h3>
<p>
	For each test case output one line containing a single integer - the number of 
	different possible sequences P.
</p>
<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
5
ab
a
a
ab
a
a
baaaa
a
a
ba

<b><tt>Sample output:</tt></b>
12
</pre>