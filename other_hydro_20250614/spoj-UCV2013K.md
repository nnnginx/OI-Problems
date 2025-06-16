<p>As many books, movies and video games had shown us, a zombie outbreak was inevitable. However, all hope is not lost. As usual you've encountered a young girl that has been bitten but not transformed. Therefore, you've escorted her to a medial facility so her blood can be studied and a cure manufactured.</p>
<p>Unfortunately, the medical facility, for obvious reasons, has not been resupplied in a while. The scientists there have asked you to pick several tools, viruses and whatnots, from N places in the city.</p>
<p>Now that you have to go out again, you have created a map with the N + 1 locations: the medical facility (location 0) and the other N where the scientists need you to pick something up (numbered from 1 to N). You've also came up with M two-way paths between some of the locations and the probability to encounter a zombie pack on each of those paths. Note that this is isn't science fiction. If you encounter a zombie pack, you will not survive.</p>
<p>You certainly want to fetch all the items and come back alive. You want to compute the maximal probability of picking every item and coming back to the medical facility (safe and sound) if you take a closed walk (cycle that allows node repetitions).</p>

<br>
<h3>Input</h3>
<p>The input contains several test cases. Each test case begins with two integers, the number of places you have to go to (1 &lt;=  N &lt;= 16) and the number of paths you came up with (1 &lt;= M &lt;= N^2), separated by a single space.</p>
<p>The next M lines contain 2 integers and a real number separated by spaces. Two integers ui and vi (0 &lt;= ui, vi &lt;=  N and ui&lt;&gt;vi) are the locations this path connects. Real number pi (0 &lt;= pi &lt;= 1) represents the probability that you will encounter a zombie pack along this path.</p>
<p>You may assume that, for all i &lt;&gt; j, probabilities pi and pj are independent from each other.</p>
<p>The end of input is indicated by a test case with N = M = 0 and should not be processed</p>

<br>
<h3>Output</h3>
<p>For each test case output a single line with a single real number: the probability of getting back to the medical facility alive with all items. Round the result to exactly three places after decimal point. If there's no way to pick all items, you should output 0.000.</p>

<br>
<h3>Example</h3>
<pre><strong>Input:</strong>
2 3<br>0 1 0.3<br>0 2 0.4<br>1 2 0.2<br>2 3<br>0 1 0.3<br>0 2 0.5<br>1 2 0.1<br>2 2<br>0 1 0.1<br>0 1 0.9<br>2 3<br>0 1 0.92<br>0 2 0.92<br>1 2 0.92<br>2 3<br>0 1 0.92<br>0 2 0.92<br>1 2 0.93<br>0 0

<strong>Output:</strong>
0.336<br>0.397<br>0.000<br>0.001<br>0.000
</pre>