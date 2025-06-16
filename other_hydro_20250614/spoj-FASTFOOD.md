<p>Hong Kil Dong wants to open a new fast food&nbsp;restaurant to make some money. The picture below describes the city where&nbsp;he wants to open&nbsp;his restaurant. The&nbsp;nodes are the possible&nbsp;locations that he can set up his new restuarant, and the edges are the&nbsp;length of the road&nbsp;connecting the&nbsp;two locations. You can assume that maximum five roads&nbsp;intersect at a single node, and that it is possible to reach&nbsp;all&nbsp;nodes&nbsp;from any chosen node.</p>
<p>There are three apartments (these three&nbsp;are the only&nbsp;places people live in)&nbsp;in this city, denoted A, B, and C, as shown in the picture.</p>
<p><img title="Graph" src="file://GVPEUb4s.png" alt="Graph" width="260" height="203"></p>
<p>Suppose he wants to open his new restuarant in location (node)&nbsp;1. The shortest distances from&nbsp;location 1 to A, B, and C are 8, 16, and 9 respectively.&nbsp;These values&nbsp;are each larger than the shortest&nbsp;distances from&nbsp;location 4 to A, B, and C, which are 6, 7, and 3. Since people usually&nbsp;prefer using&nbsp;closer restuarants, it is better to open his restaurant in&nbsp;location 4.</p>
<p>Consider&nbsp;location 6. The shortest&nbsp;distances from&nbsp;location 6 to A,&nbsp;B, and C are 5, 3, and 5.&nbsp;Therefore,&nbsp;location 6 is better than location 1. However,&nbsp;when comparing&nbsp;with location 4, it is better regarding&nbsp;A and B, but worse&nbsp;when considering&nbsp;C.</p>
<p>Therefore, Hong Kil Dong came up with a&nbsp;criteria to determine whether a given&nbsp;location is good or bad.</p>
<p>Consider location p, and let&nbsp;the shortest&nbsp;distances from location p to A, B, and C be a, b, and c, respectively.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>Consider another&nbsp;location q, and let the shortest&nbsp;distances from location q to A, B, and C be x, y, z, respectively.</p>
<p>If a&gt;x, b&gt;y and c&gt;z, we say that location p is a bad location. If there is no location q that satisfies this, we say that location p is a good location.</p>
<p>Hong Kil Dong has chosen some candidate locations. Given the description of the city and a number of queries, determine whether&nbsp;each&nbsp;candidate location is good or bad.</p>
<p>Note that it is possible to open the restaurant in any of the locations, even in &nbsp;A, B, and C.</p>
<h3>Input</h3>
<p>The first line of the input is an integer N (1&lt;=N&lt;=100,000), denoting the number of locations. &nbsp;All the locations are numbered from 1-N.</p>
<p>The second line of the input is three integers A, B, and C, denoting the location of each apartment. A, B, and C are all&nbsp;distinct and are between 1 and N, inclusive.</p>
<p>The third line of the input is M, denoting the number of roads in this city.</p>
<p>The next M lines give the description of each road and consist of integer X, Y, and Z (1&lt;=Z&lt;=10,000). X and Y are the two endpoints of this road, and Z is the length of this road. No two same roads appear in the input.</p>
<p>The next line is an integer T (1&lt;=T&lt;=10,000), denoting the number of queries.</p>
<p>The next&nbsp;T lines&nbsp;each consist of an integer Q (1&lt;=Q&lt;=N), which denote the location number.&nbsp;</p>
<h3>Output</h3>
<p>For each query, determine whether location Q is a good location or a bad location. If it is bad, output "NO" (quotes for clarity) and "YES" if it is good.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
9<br>2 5 9<br>15<br>1 2 8<br>1 3 5<br>2 4 6<br>2 5 8<br>2 6 5<br>3 4 6<br>3 9 4<br>4 6 4<br>4 9 3<br>5 6 3<br>5 7 4<br>6 7 2<br>6 9 5<br>7 8 7<br>8 9 6<br>2<br>1<br>2<br>
<strong>Output:</strong>
NO<br>YES<br>
</pre>