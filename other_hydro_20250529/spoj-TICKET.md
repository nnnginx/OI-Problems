<p>
<img src="./24668/file/NyASLs0C.png">
</p>
<p>
Ticket to Ride is a board game for up to 5 players.  The goal of the
game is to set up train lines (and to thwart the opponents' attempts
at setting up their train lines).  At the beginning of play, each
player is assigned four train lines.  A player may choose to discard
as many of these four assignments as she likes.  Each assignment has a
score, corresponding to its difficulty (so, typically, a train line
between e.g. Stockholm and Tokyo would be worth more than a train
line between e.g. Stockholm and Utrecht).  At the end of the game,
each player gets points for the assignments that they have
successfully completed, and penalty points for the assignments that
they have failed to complete.

</p><p>
An assignment consists of a pair of cities that are to be connected by
a series of shorter railway routes.  A route can be claimed (for a
certain cost associated with the route), but things are complicated by
the fact that there is only a limited number of routes, and once a player
claims a route, none of the other players can claim it.  A player has
successfully set up a train line between two cities if there is a path
between the two cities using only routes that have been claimed by
this player.  For simplicity, we will ignore all additional aspects of
the game (including the actual process of claiming routes and
additional ways to score points).
</p>
<p>
For instance, if your assignment is to connect Stockholm and Amsterdam
in the Figure above, you would probably want to claim the routes
between Stockholm and Copenhagen, and between Copenhagen and
Amsterdam.  But if another player manages to claim the route between
Copenhagen and Stockholm before you, your train line would have to use
some other routes, e.g. by going to Copenhagen via Oslo.
</p>
<p>
In this problem, we will consider the rather bold strategy of trying
to complete all four assignments (typically, this will be quite
hard).  As a preliminary assessment of the difficulty of achieving
this, we would like to calculate the minimum cost of setting up all
four lines assuming that none of the other players interfere with our
plans.  Your job is to write a program to determine this minimum cost.
</p>
<h3>Input</h3>
<p>
The input consists of several (at most 20) games to be analyzed.  Each
game starts with two integers 1 �� <em>n</em> �� 30, 0 ��

<em>m</em> �� 1000, giving the number of cities and railway routes
in the map, respectively.  Then follow <em>n</em> lines, giving the
names of the <em>n</em> cities.  City names are at most 20 characters
long and consist solely of lower case letters
(<tt>'a'-'z'</tt>).
</p>
<p>
After this follow <em>m</em> lines, each containing the names of two
different cities and an integer 1 �� <em>c</em> �� 10000,
indicating that there is a railway route with cost <em>c</em> between
the two cities.  Note that there may be several railway routes between
the same pair of cities.  You may assume that it is always possible to
set up a train line from any city to any other city.
</p>

<p>
Finally, there will be four lines, each containing the names of two
cities, giving the four train line assignments.
</p>
<p>
The input is terminated by a case where <em>n</em> = <em>m</em> = 0.
This case should not be processed.
</p>
<h3>Output</h3>
<p>
For each game, output a single line containing a single integer, the
minimum possible cost to set up all four train lines.
</p>
<h3>Example</h3>

<pre><b>Input:</b>
10 15
stockholm
amsterdam
london
berlin
copenhagen
oslo
helsinki
dublin
reykjavik
brussels
oslo stockholm 415
stockholm helsinki 396
oslo london 1153
oslo copenhagen 485
stockholm copenhagen 522
copenhagen berlin 354
copenhagen amsterdam 622
helsinki berlin 1107
london amsterdam 356
berlin amsterdam 575
london dublin 463
reykjavik dublin 1498
reykjavik oslo 1748
london brussels 318
brussels amsterdam 173
stockholm amsterdam
oslo london
reykjavik dublin
brussels helsinki
2 1
first
second
first second 10
first first
first first
second first
first first
0 0

<b>Output:</b>
3907
10
</pre>