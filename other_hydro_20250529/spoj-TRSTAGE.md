<p>Once upon a time, there was a traveler.

<br><br>
He plans to travel using stagecoaches (horse wagons). His starting point and destination are fixed, but he cannot determine his route. Your job in this problem is to write a program which determines the route for him.

<br><br>
There are several cities in the country, and a road network connecting them. If there is a road between two cities, one can travel by a stagecoach from one of them to the other. A coach ticket is needed for a coach ride. The number of horses is specified in each of the tickets. Of course, with more horses, the coach runs faster.

<br><br>
At the starting point, the traveler has a number of coach tickets. By considering these tickets and the information on the road network, you should find the best possible route that takes him to the destination in the shortest time. The usage of coach tickets should be taken into account.

<br><br>
The following conditions are assumed.

<br><br>
</p><ul>
<li> A coach ride takes the traveler from one city to another directly connected by a road. In other words, on each arrival to a city, he must change the coach.
</li><li> Only one ticket can be used for a coach ride between two cities directly connected by a road.
</li><li> Each ticket can be used only once.
</li><li> The time needed for a coach ride is the distance between two cities divided by the number of horses.
</li><li> The time needed for the coach change should be ignored. 
</li></ul>

<br><br>
<h3>Input</h3>
<p>The input consists of multiple datasets, each in the following format. The last dataset is followed by a line containing five zeros (separated by a space).

<br><br>
    n m p a b<br>
    t1 t2 ... tn<br>
    x1 y1 z1<br>
    x2 y2 z2<br>
    ...<br>
    xp yp zp<br>

<br><br>
Every input item in a dataset is a non-negative integer. If a line contains two or more input items, they are separated by a space.<br>

<br>
n is the number of coach tickets. You can assume that the number of tickets is between 1 and 8. m is the number of cities in the network. You can assume that the number of cities is between 2 and 30. p is the number of roads between cities, which may be zero.

<br><br>
a is the city index of the starting city. b is the city index of the destination city. a is not equal to b. You can assume that all city indices in a dataset (including the above two) are between 1 and m.

<br><br>
The second line of a dataset gives the details of coach tickets. ti is the number of horses specified in the i-th coach ticket (1&lt;=i&lt;=n). You can assume that the number of horses is between 1 and 10.

<br><br>
The following p lines give the details of roads between cities. The i-th road connects two cities with city indices xi and yi, and has a distance zi (1&lt;=i&lt;=p). You can assume that the distance is between 1 and 100.

<br><br>
No two roads connect the same pair of cities. A road never connects a city with itself. Each road can be traveled in both directions. 

<br>
</p><h3>Output</h3>
<p> For each dataset in the input, one line should be output as specified below. An output line should not contain extra characters such as spaces.

<br><br>
If the traveler can reach the destination, the time needed for the best route (a route with the shortest time) should be printed. The answer should not have an error greater than 0.001. You may output any number of digits after the decimal point, provided that the above accuracy condition is satisfied.

<br><br>
If the traveler cannot reach the destination, the string "Impossible" should be printed. One cannot reach the destination either when there are no routes leading to the destination, or when the number of tickets is not sufficient. Note that the first letter of "Impossible" is in uppercase, while the other letters are in lowercase. 

<br>
</p><h3>Example</h3>

<pre><b>Input:</b>
3 4 3 1 4
3 1 2
1 2 10
2 3 30
3 4 20
2 4 4 2 1
3 1
2 3 3
1 3 3
4 1 2
4 2 5
2 4 3 4 1
5 5
1 2 10
2 3 10
3 4 10
1 2 0 1 2
1
8 5 10 1 5
2 7 1 8 4 5 6 3
1 2 5
2 3 4
3 4 7
4 5 3
1 3 25
2 4 23
3 5 22
1 4 45
2 5 51
1 5 99
0 0 0 0 0

<b>Output:</b>
30.000
3.667
Impossible
Impossible
2.856

Since the number of digits after the decimal point is
not specified, the above result is not the only
solution. For example, the following result is also acceptable.

30.0
3.66667
Impossible
Impossible
2.85595
</pre>