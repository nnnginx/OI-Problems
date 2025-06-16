<p style="text-align: justify;">Little Johnny has got a new car. He decided to drive around the town to visit his friends. Johnny wanted to visit all his friends, but there was many of them. In each street he had one friend. He started thinking how to make his trip as short as possible. Very soon he realized that the best way to do it was to travel through each street of town only once. Naturally, he wanted to finish his trip at the same place he started, at his parents' house.</p>
<p style="text-align: justify;">The streets in Johnny's town were named by integer numbers from 1 to&nbsp;<em>n</em>,&nbsp;<em>n</em>&nbsp;&lt; 1995. The junctions were independently named by integer numbers from 1 to&nbsp;<em>m</em>,&nbsp;<img src="./23020/file/KiwpXMux.png" alt="tex2html_wrap_inline32" width="54" height="25" align="MIDDLE">&nbsp;. All junctions in the town had different numbers. Each street was connecting exactly two (not necessarily different) junctions. No two streets in the town had the same number. He immediately started to plan his round trip. If there was more than one such round trip, he would have chosen the one which, when written down as a sequence of street numbers is lexicographically the smallest.</p>
<p style="text-align: justify;">But Johnny was not able to find even one such round trip. Help Johnny and write a program which finds the desired shortest round trip. If the round trip does not exist the program should write a message. Assume that Johnny lives at the junction ending the 1st street input with smaller number. All streets in the town are two way. There exists a way from each street to another street in the town. The streets in the town are very narrow and there is no possibility to turn back the car once he is in the street.</p>
<p>&nbsp;</p>
<h2><span style="color: #000000;"><a name="SECTION0001001000000000000000">Input</a></span></h2>
<p style="text-align: justify;">Input file consists of several blocks. Each block describes one town. Each line in the block contains three integers&nbsp;<em>x</em>,&nbsp;<em>y</em>,&nbsp;<em>z</em>, where&nbsp;<em>x</em>&nbsp;&gt; 0 and&nbsp;<em>y</em>&nbsp;&gt; 0 are the numbers of junctions which are connected by the street number&nbsp;<em>z</em>. The end of the block is marked by the line containing&nbsp;<em>x</em>&nbsp;=&nbsp;<em>y</em>&nbsp;= 0. At the end of the input file there is an empty block,&nbsp;<em>x</em>&nbsp;=&nbsp;<em>y</em>&nbsp;= 0.</p>
<p style="text-align: justify;">&nbsp;</p>
<h2><span style="color: #000000;"><a name="SECTION0001002000000000000000">Output</a></span></h2>
<p style="text-align: justify;">The output file consists of 2 line blocks corresponding to the blocks of the input file. The first line of each block contains the sequence of street numbers (single members of the sequence are separated by space) describing Johnny's round trip. If the round trip cannot be found the corresponding output block contains the message ``<tt>Round trip does not exist.</tt>''. The second line of each block is empty.</p>
<p style="text-align: justify;">&nbsp;</p>
<h2><span style="color: #000000;"><a name="SECTION0001003000000000000000">Sample Input</a></span></h2>
<pre>1 2 1
2 3 2
3 1 6
1 2 5
2 3 3
3 1 4
0 0
1 2 1
2 3 2
1 3 3
2 4 4
0 0
0 0</pre>
<p>&nbsp;</p>
<h2><span style="color: #000000;"><a name="SECTION0001004000000000000000">Sample Output</a></span></h2>
<pre>1 2 3 5 4 6

Round trip does not exist.</pre>