<p>Rand has been sitting in a spaceship at the point (0,0,0) for a long time. One day, he got bored and decided to undertake an adventure.</p>
<p>Deciding upon an adventure has several complicated steps. First, Rand chooses a destination point (x,y,z) different from (0,0,0) such that 0&lt;=x&lt;=A, 0&lt;=y&lt;=B, 0&lt;=z&lt;=C. To go to this point, Rand travels in a straight line from the origin. As a result, he might encounter several other lattice points in the way. Each part of the journey between two consecutive lattice points encountered is called a phase.( For example if (x,y,z)=(1,2,3) then there is only one phase (0,0,0)-&gt;(1,2,3), while if (x,y,z)=(3,0,3) then there are 3 phases (0,0,0)-&gt;(1,0,1)-&gt;(2,0,2)-&gt;(3,0,3) ).</p>
<p>In each phase Rand chooses one of K different activities that he can undertake to pass the time. You need to calculate the total number of different adventures possible, modulo 1000000007 (1e9+7). Two adventures are considered different if they have different destination points, or if the activity undertaken during any of the corresponding phases is different.</p>
<h3>Input</h3>
<p>The first line contains the number T, the number of test cases.<br>T lines follow, each contains the integers A,B,C,K, corresponding to one testcase</p>
<h3>Output</h3>
<p>Output T lines, each with one integer as the answer for the corresponding test case.</p>
<h3>Constraints</h3>
<p>T &lt;= 1000<br>0 &lt;= A,B,C &lt;= 50000<br>1 &lt;= K &lt;= 10</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3<br>0 0 5 2<br>0 2 2 5<br>4 4 4 9

<strong>Output:</strong>
62<br>100<br>53388<br><br></pre>
<h3>Explanation</h3>
<p>In the first test case, if Rand chooses (0,0,1) as destination point, then there are 2 possible adventures. Similarly for (0,0,2), (0,0,3), (0,0,4) and (0,0,5), the number of adventures corresponding to each are 4,8,16,32 respectively. The total number of adventures is 2+4+8+16+32=62.</p>
<p>In the second test case, for points (0,0,2), (0,2,0) and (0,2,2) there are 25 adventures each, while for the rest of the 5 valid points, there are 5 adventures each. So total is 100.</p>