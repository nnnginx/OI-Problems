<p align="justify">
Write a program that finds all occurences of a given pattern in a given input string. This is often referred to as finding a <em>needle</em> in a <em>haystack</em>.</p>
<p>The program has to detect <strong>all</strong> occurences of the needle in the haystack. It should take the needle and the haystack as input, and output the positions of each occurence, as shown below.
The suggested implementation is the KMP algorithm, but this is not a requirement. However, a naive approach will probably exceed the time limit, whereas other algorithms are more complicated... The choice is yours.</p>
<h3>Input</h3>
<p>The input consists of a number of test cases. Each test case is composed of three lines, containing:</p>
<div align="left">
<ul>
	<li>the length of the needle,</li>
	<li>the needle itself,</li>
	<li>the haystack.</li>
</ul>
</div>
<p>The length of the needle is only limited by the memory available to your program, so do not make any assumptions - instead, read the length and allocate memory as needed. The haystack is <strong>not</strong> limited in size, which implies that your program should not read the whole haystack at once. The KMP algorithm is stream-based, i.e. it processes the haystack character by character, so this is not a problem.</p>
<p>The test cases come one after another, each occupying three lines, with no additional space or line breaks in between.</p>
<h3>Output</h3>
<p>For each test case your program should output all positions of the needle's occurences within the haystack. If a match is found, the output should contain the position of the first character of the match. Characters in the haystack are numbered starting with zero.</p>
<p>For a given test case, the positions output should be sorted in ascending order, and each of these should be printed in a separate line. For two different test cases, the positions should be separated by an empty line.</p>
<h3>Example</h3>
<pre><b>Sample input:</b>
2
na
banananobano
6
foobar
foo
9
foobarfoo
barfoobarfoobarfoobarfoobarfoo</pre>

<pre><b>Sample output:</b>
2
4

3
9
15
21
</pre>
<p>Note the double empty line in the output, which means that no match was found for the second test case.</p>
<b>Warning: large Input/Output data, be careful with certain languages</b>