<p>Please click <a href="http://www.spoj.com/content/john_jones:shanghai2009.pdf">here</a> to download a PDF version of the contest problems. The problem is problem B in the PDF. But the data limits is slightly modified: 1¡ÜP¡Ü1000000 in the original description, but in this EXTREME version, 1¡ÜP¡Ü1000000000.</p>
<pre>=========(EDIT, Francky)===============</pre>
<p>Professor Brute is not good at algorithm design. Once he was asked to solve a path finding problem. He worked on it for several days and finally came up with the following algorithm:</p>
<pre>Function Find(integer n,function func)
	If n=1
		For i = 1 to a do func()
	Elseif n=2
		For i = 1 to b do func()
	Else Find(n-1,Find(n-2,func))
Function Main
	Find(n,funny)
</pre>
<p>Any fool but Brute knows that the function ¡°funny¡± will be called too many times. Brute wants to investigate the number of times the function will be called, but he is too lazy to do it.<br> Now your task is to calculate how many times the function ¡°funny¡± will be called, for the given a, b and n. Because the answer may be too large, you should output the answer module by P.</p>
<h3>Input</h3>
<p>There are multiple test cases. The first line of the input contains an integer T, meaning the number of the test cases.<br> For each test cases, there are four integers a, b, P and n in a single line. You can assume that 1¡Ün¡Ü1000000000, 1¡ÜP¡Ü1000000, 0¡Üa, b&lt;1000000.</p>
<h3>Output</h3>
<p>For each test case, output the answer with case number in a single line.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
3 4 10 3
4 5 13 5
3 2 19 100

<strong>Output:</strong>
Case #1: 2
Case #2: 11
Case #3: 12
</pre>