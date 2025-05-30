<p>Mr. B is an airport manager. One day after lunch he looked out from his office and found that the color of each plane   which was currently parked in the airport is either blue or green. Before supper he found that no plane is on the airport   now. He couldn't remember the orders in which the planes took off, but he knew between the two observations no plane arrived   at the airport. In addition, while one plane is setting its way to the takeoff area, the remaining planes must stay at their   own position and cannot move. In the other words, considering the planes taking off in a specific order, the first plane will   move while others stay at their own position. After the first plane took off, the second plane could move to the takeoff area   and so on, until all the planes gone. Now he wants you to find out the number of different possible color sequences he might   see, if he watched at the takeoff area during the whole afternoon.</p>
<p>The airport can be divided into 9 square areas (3 rows x 3 columns), each area can park at most one plane. The area   located at the first column of the first row is called "takeoff area". The plane can take off only in the takeoff area.   Besides, each plane (including the one in the takeoff area) can move to a vacant neighboring area. Two areas are neighboring   if and only if they share an edge.</p>
<h3>Input</h3>
<p>Each test case contains 3 lines, each of which contains 3 characters '*', 'B', 'G', denoting that the corresponding area   is currently vacant, occupied by a blue plane, or occupied by a green plane, respectively. The first character of the first   row is always a '*'. </p>
<p>There are about 30,000 test cases. Be careful!</p>
<h3>Output</h3>
<p>For each test case, display a single line containing the case number and the number of different possible color sequences   Mr. B might see.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
*BB
BBB
BBB
*GB
BBB
BBB

<strong>Output:</strong>
Case 1: 1
Case 2: 8
</pre>