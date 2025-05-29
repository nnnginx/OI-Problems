<p>My kid's kindergarten class is putting up a Christmas play.&nbsp; (I hope he gets the lead role.)&nbsp; The kids are all excited, but the teacher has a lot of work.&nbsp; She has to produce costumes for a scene with K soldiers.&nbsp; She wants to buy all the costumes in the same size, allowing for some small amount of length alteration to be done by the kids' parents later.&nbsp; So she has taken all the kids' height measurements.&nbsp; Can you help her select K kids from her class of N to play the soldier role, such that the height difference between the tallest and shortest in the group is minimized, and alternations will be easiest?&nbsp; Tell her what this minimum difference is. <br>&nbsp;<br>&nbsp;<br><strong>INPUT</strong> <br>The first line contains the number of test cases T. T test cases follow each containing 2 lines. <br>&nbsp;<br>The first line of each test case contains 2 integers N and K. <br>The second line contains N integers denoting the height of the N kids. <br>&nbsp;<br><strong>OUTPUT</strong> <br>Output T lines, each line containing the required answer for the corresponding test case. <br>&nbsp;<br><strong>CONSTRAINTS</strong> <br>T &lt;= 30 <br>1 &lt;= K &lt;= N &lt;= 20000 <br>1 &lt;= height &lt;= 1000000000 <br>&nbsp;<br>

<strong>SAMPLE INPUT</strong>
</p><pre>3
3 1
2 5 4
3 2
5 2 4
3 3
2 5 4</pre>

<strong>SAMPLE OUTPUT</strong>
<pre>0
1
3</pre>

<strong>EXPLANATION</strong><br>In the first test case, the teacher needs to only select 1 kid and hence she can choose any kid since the height difference is going to be 0. <br>In the second test case, the teacher can choose kids with height 4 and 5. <br>In the third test case, the teacher is forced to choose all 3 kids and hence the answer = 5-2 = 3<p></p>