<p>Thor, the Norse god of thunder, was shopping for groceries when he noticed a sale on Kleenex brand tissues. This got him thinking about Kleene¡¯s recursion theorem and its application to quines in functional programming languages. As this gave him a headache, he instead turned his attention to how one might recognise regular expressions with Kleene stars on a Turing machine. Unfortunately, this just made his headache worse. So he took out a slip of paper, jotted down a brainf**k program to handle regular expressions containing Kleene plusses, paid for his groceries, and congratulated himself on a job well done.</p>
<p><strong>Note:</strong> You can use any programming language you want, as long as it is brainf**k.</p>
<h3>Input</h3>
<p>The first line contains an integer <strong>T</strong> (1 ¡Ü <strong>T</strong> ¡Ü 1000). Then follow <strong>T</strong> test cases.
</p><p>For each test case: The first line contains a regular expression <strong>P</strong> (1 ¡Ü |<strong>P</strong>| ¡Ü 30). The next line contains an integer <strong>Q</strong> (1 ¡Ü <strong>Q</strong> ¡Ü 10). Then follow <strong>Q</strong> lines, each containing a string <strong>S</strong> (1 ¡Ü |<strong>S</strong>| ¡Ü 100). Finally, there is an empty line at the end of each test case.</p>
<p>Each line, including the last, is terminated by a single newline (linefeed) character, which has ASCII value 10.</p>
<p>All regular expressions are guaranteed to be valid; in particular, <strong>P</strong> may not start with a plus, and it may not contain two consecutive plusses. <strong>P</strong> is a string over the alphabet {a,b,c,d,+}, and <strong>S</strong> is a string over the alphabet {a,b,c,d}.</p>
<h3>Output</h3>
<p><strong>T</strong> lines each containing a string of length <strong>Q</strong>. The <strong>i</strong>th character of the string indicates whether <strong>S</strong> is in the regular language defined by <strong>P</strong>: 'Y' for a match, and '.' otherwise. Note that we are concerned whether <strong>P</strong> matches <strong>S</strong>, as opposed to a substring of <strong>S</strong>. In other words, we could insert '^' at the beginning of <strong>P</strong> and '$' at the end, and then test for a match using e.g. m// in Perl. See the example for further clarification.</p>
<h3>Example</h3>
<p><strong>Input:</strong></p>
<pre>3
a
2
a
aa

a+
2
a
aa

a+bc
6
abbacadabba
aaaabc
abc
bc
abcd
babc

</pre>
<p><strong>Output:</strong></p>
<pre>Y.
YY
.YY...
</pre>
<h3>Additional Info</h3>
<p>There are two randomly generated data sets, one with <strong>T</strong>=1000 and the other with <strong>T</strong>=500. The average value of <strong>Q</strong> is about 6, the probability of a match is about 0.25, the average length of <strong>P</strong> is about 14, and the average length of <strong>S</strong> is about 27.</p>
<p>My solution at the time of publication has 803 bytes (not golfed) and runs in 0.20s with 2.6M memory footprint.</p>