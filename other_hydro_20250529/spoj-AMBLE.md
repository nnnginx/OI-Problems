<p>Alicia is staying in a hotel on the edge of town. She sets out in the morning with a list of landmarks to visit all across the city. This day of sightseeing will take her through the city, visiting a number of locations, all the way to the far-side of city where she will pause for lunch at the prestigious Pete¡¯s Polygon Pizza Parlour. Anything she misses must be visited on the return trip to the hotel in the evening.</p>
<p>Given the set of locations that Alicia would like to visit, find the length of the shortest tour which starts at her hotel, visits each of the locations, and returns back to the hotel. Beside the starting location, each location should be visited exactly once.</p>
<p>The starting hotel will be located at the leftmost x-coordinate. From there, the optimal path should visit locations at strictly increasing x-coordinates until Pete¡¯s Parlour is reached at the rightmost x-coordinate. From here, the optimal return path should visit any and all unseen locations in strictly decreasing x-coordinates.</p>
<p>Note that the x-coordinate of each location will be unique.</p>
<h3>Input</h3>
<p>The first line of input contains a single integer N, 1 ¡Ü N ¡Ü 1000, representing the number of locations.</p>
<p>Each of the next n lines contains two integers X and Y, 0 ¡Ü X, Y ¡Ü 100000, representing the coordinates of the N locations.</p>
<p>The (X, Y) coordinates of all locations are given as integers on a Euclidean plane.</p>
<h3>Output</h3>
<p>The output should consist of a single decimal containing the the total length of the tour rounded to two decimal places. This should immediately be followed by a newline.</p>
<h3><span style="font-size: 1.17em;">Example One</span></h3>
<pre><strong>Input:</strong>
5&nbsp;<br>1 3<br>2 1<br>3 4<br>4 4<br>5 2&nbsp;</pre>
<pre><strong>Output:</strong>
10.87</pre>
<h3>Example Two</h3>
<pre><strong>Input:</strong>
10<br>4 1<br>13 4<br>21 3<br>25 9<br>28 10<br>42 1<br>43 2<br>50 4<br>67 10<br>68 9</pre>
<pre><strong>Output:</strong>
131.65</pre>