<p>Members of the famous ENSI Competitive Programming Club try to gather a huge database of problem sets. They need to sort all the problems according to their difficulty levels. Each of the M club members takes N problems and brings back the sorted list. The score (difficulty level) is a real value evaluated as a combination of many criterions. Write a program that outputs the global sorted list of N*M problems.</p>
<h3>Input</h3>
<p>First line of input consists of an integer T denoting the number of test cases. Then T test cases follow. Each case begins with two lines containing two integers M and N (N*M&lt;=10^6). Each of the M next lines contains N space separated real numbers (scores) in descending order. All the scores are guaranteed to be in [0, 10].</p>
<h3>Output</h3>
<p>A single line for each test case consisting of N*M space separeted problems.  Each problem is represented by i,j where i is the input member position (from 1 to M) and j is the position in the original list (from 1 to N). Problems are sorted by score (descending order) then by member's position (ascending order) and finally by problem's position in the original member¡¯s list (ascending order).</p>
<p><span style="text-decoration: underline;"><strong>Input File is large. Use fast I/O methods.</strong></span></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
3 
4
9.195 4.17 2.532 0.03
8.28 5.5 4 2.69 
8.8320 7.9 2.18 0
 
<strong>Output:</strong>
1,1 3,1 2,1 3,2 2,2 1,2 2,3 2,4 1,3 3,3 1,4 3,4</pre>
<p>&nbsp;</p>