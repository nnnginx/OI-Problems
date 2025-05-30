<p>Boy Scouts of New England organize Scout Olympics every year. They
ask each team to perform certain tasks, sum up their points, announce
winners, and then stay up all night by the fire plying guitar and
singing scout songs.

This year, Scouts decided to organize the Olympics in one of the most
beautiful forests in Maine. There will be only one difficult task.
A team picks one tree as a starting point, then goes to another tree
in a straight line, then to another, etc. until they come back to the
starting one. They win as many points as there are trees on their route.
However, they are only allowed to move in a counter-clockwise manner,
i.e. after reaching a tree, they can only rotate to the left by less than 180
degrees. Furthermore, when they reach the starting tree again, they
should be able to repeat the same route, still going couter-clockwise. More specifically, their path should trace out the boundary of a convex polygon.

As they don't bring laptops to the Olympics, the Boy Scouts wants you to compute
the maximum possible score a team can achieve.

</p><h3>Input</h3>
<p>The first line of the input contains a single integer N (3 �� N �� 100),
which is the number of trees in the forest. Each of the next N lines
contain two real numbers x and y separated by a space character
(-10<sup>6</sup> �� x, y �� 10<sup>6</sup>), that represent coordinates of one tree.
Coordinates are given with at most two decimal digits. There are no three
colinear trees.

</p><h3>Output</h3>
<p>Output one integer, the maximum number of points a team can score, followed
by a newline.

</p><h3>Example</h3>

<pre><b>Input:</b>
5
0 0
1.5 -0.25
0 -1
-1 0.5
0.5 1

<b>Output:</b>
4
</pre>