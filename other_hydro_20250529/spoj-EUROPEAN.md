<p>As you may already know, different countries in Europe use different railroad systems. Not only do they use different voltages for their trains, but also the distance between the two rails (gauge) differs. The following table shows some railway gauges used:</p>
<table class="data" border="1" cellspacing="1" cellpadding="1">
<tbody>
<tr>
<th>Broad gauge (Spain):</th> <th>1674 mm</th>
</tr>
<tr>
<th>Broad gauge (Portugal):</th> <th>1665 mm</th>
</tr>
<tr>
<th>Broad gauge (Ireland):</th> <th>1600 mm</th>
</tr>
<tr>
<th>Broad gauge (Finland):</th> <th>1524 mm</th>
</tr>
<tr>
<th>Broad gauge (former USSR):</th> <th>1520 mm</th>
</tr>
<tr>
<th>Standard gauge:</th> <th>1435 mm</th>
</tr>
<tr>
<th>Narrow gauge (meter gauge):</th> <th>1000 mm</th>
</tr>
</tbody>
</table>
<p>A museum has trains from several countries. It needs tracks for every train type in order to show visitors the trains in use. However, since only one train is used at a time, a rail can be used by trains of different types. It follows that for <em>n</em> trains, each requiring a different railway gauge, <em>n + 1</em> rails are sufficient (each train uses the leftmost rail and a rail that has exactly the required distance to it). But sometimes it is possible to save even more rails.</p>
<p>Given the required railway gauges, your task is to construct a railway track that can be used by every train and requires the least number of rails. Note that a train can use any two rails, provided the distance between them is right.</p>
<h3>Input Specification</h3>
<p>The first line of the input file contains a number representing the number of test cases to follow. Each test case starts with an integer <em>n</em> (the number of different railway gauges required). The next line contains <em>n</em> integers between <em>1000</em> and <em>5000</em>, each defining one required railway gauge.<br> You can assume that <em>1 �� n �� 8</em>. Moreover, for every test case in the input file, there will be a solution requiring at most <em>5</em> rails.</p>
<h3>Output Specification</h3>
<p>The output for each test case consists of three lines:<br> The first line is of the form "Scenario #X", where X is the test case number starting with 1. The second line describes the solution your program has found; first your program should print how many rails are needed, followed by a colon, then the positions of each rail in increasing order (the first rail should be at position 0). The third line should be blank. If there are several solutions with the minimum number of rails, any one will do.</p>
<h3>Sample Input</h3>
<pre>3
4
1524 1520 1609 1435
3
1000 1520 1600
6
1000 2000 3000 4000 1500 2500
</pre>
<h3>Sample Output</h3>
<pre>Scenario #1
4: 0 1520 1609 3044

Scenario #2
4: 0 1000 1520 1600

Scenario #3
5: 0 1500 3000 4000 5000

</pre>