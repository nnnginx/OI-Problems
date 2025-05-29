<p><em>Original statement in spanish at <a href="http://www.dc.uba.ar/events/icpc/download/problems/taip2011-problems.pdf">http://www.dc.uba.ar/events/icpc/download/problems/taip2011-problems.pdf</a></em></p>
<p>Everyone is aware of the existence of the well known Nordenskjold  Archipelago, located in the Arctic Ocean and belonging to the  Krasnoyarsk Krai of Russia. This archipelago  consists of a groups of <strong>N</strong> islands and <strong>M</strong> aquatic routes between some  pairs of islands. Each route connects a pair of islands and for each  pair there is at most one route connecting them.</p>
<p>Considering the popularity of Nordenskjold Archipelago,  Krasnoyarsk's authorities are concerned about its touristic value. The  touristic value of the archipelago is given by the total number of  islands that belong to at least one ��touristic circuit��.  A touristic circuit is a path starting and ending in the same island  that visits at least three different islands, never visits the same  island more than once and uses just aquatic routes to go from one  island to the next one.</p>
<p>Krasnoyarsk's authorities want to know the minimum number of  additional aquatic routes that must be built so that every  island belongs to at least one touristic circuit. Your task is to  write a program that answers this question.</p>
<h3>Input</h3>
<p>The input contains several test cases. Each test case is described  in several lines. The first line contains two integer numbers <strong>N</strong> and <strong>M</strong> (3 &lt;= <strong>N</strong> &lt;= 100, 1 &lt;= <strong>M</strong> &lt;= 1000) which indicate the number  of islands and the number of aquatic routes, respectively. Each  island is identified by a number between 1 and <strong>N</strong>. Each of the next <strong>M</strong> lines contains two integers <strong>U</strong> and <strong>V</strong> (1 &lt;= <strong>U</strong> &lt; <strong>V</strong> &lt;= <strong>N</strong>),  indicating that there is an aquatic route connecting islands <strong>U</strong> and <strong>V</strong>.  You may assume that in each test case there is at most one aquatic  route connecting the same pair of islands. The last line of the input  contains the number -1 twice and should not be processed as a test case.</p>
<h3>Output</h3>
<p>For each test case output a single line with an integer  representing the  minimum number of  additional aquatic routes that must be built so that every  island belongs to at least one touristic circuit.</p>
<h3>Example</h3>
<p><strong>Input:</strong></p>
<pre>3 1
1 3
9 10
1 2
2 3
1 3
7 9
5 9
5 7
6 8
4 6
4 8
8 9
4 4
1 2
1 4
1 3
2 3
12 9
1 7
2 6
4 9
9 10
8 12
1 5
1 8
8 11
4 10
-1 -1</pre>
<p><strong>Output:</strong></p>
<pre>2
0
1
4</pre>