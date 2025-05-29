<p>Farmer John is making the difficult transition from raising mountain
goats to raising cows.  His farm, while ideal for mountain goats,
is far too mountainous for cattle and thus needs to be flattened
out a bit. Since flattening is an expensive operation, he wants to
remove the smallest amount of earth possible.
</p><p>
The farm is long and narrow and is described in a sort of two-dimensional
profile by a single array of N (1 &lt;= N &lt;= 1000) integer elevations
(range 1..1,000,000) like this:
</p><p>
1 2 3 3 3 2 1 3 2 2 1 2,
</p><p>
which represents the farm's elevations in profile, depicted below
with asterisks indicating the heights:
</p><pre>    * * *     *
  * * * * *   * * *   *
* * * * * * * * * * * *
1 2 3 3 3 2 1 3 2 2 1 2
</pre>
<p>
A contiguous range of one or more equal elevations in this array
is a "peak" if both the left and right hand sides of the range are
either the boundary of the array or an element that is lower in
elevation than the peak. The example above has three peaks.
</p><p>
Determine the minimum volume of earth (each unit elevation reduction
counts as one unit of volume) that must be removed so that the
resulting landscape has no more than K (1 &lt;= K &lt;= 25) peaks.  Note
well that elevations can be reduced but can never be increased.
</p><p>
If the example above is to be reduced to 1 peak, the optimal solution
is to remove 2 + 1 + 1 + 1 = 5 units of earth to obtain this set
of elevations:
</p><pre>    * * *     -
  * * * * *   - - -   -
* * * * * * * * * * * *
1 2 3 3 3 2 1 1 1 1 1 1
</pre>
<p>
where '-'s indicate removed earth.

</p><h3>Input</h3>
<p>
The first line of the input contains integer t representing the number of test cases. Then t test cases follow. Each test case has the following form:
</p><ul>
<li> Line 1: Two space-separated integers: N and K

</li><li> Lines 2..N+1: Each line contains a single integer elevation. Line
        i+1 contains the elevation for index i.
</li></ul>
<h3>Output</h3>
<p>For each test case, output the minimum volume of earth that must be removed to reduce
        the number of peaks to K.

</p><h3>Example</h3>

<pre><b>Input:</b>
1
12 1
1
2
3
3
3
2
1
3
2
2
1
2

<b>Output:</b>
5

<b>Input details</b>
This is the example used above.
</pre>