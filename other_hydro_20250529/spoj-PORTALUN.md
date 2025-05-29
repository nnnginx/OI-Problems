<p>You, as the newly recruited mad scientist at Aperture Laboratories, has been challenged by GLaDOS to a game that will test a new type of Portal! The invention is a series of portals, to each of which is assigned a priority.</p>
<p>One can only move from a portal with higher priority to another with lower priority. The game consists of moving the test subjects through the rooms of Aperture Science Enrichment Center. You and GLaDOS alternate turns: at each turn a player must move one of the subjects to a new room using the new portal prototype. Since her disastrous experiment with Chell, GLaDOS has decided not to hand over handheld portal devices to guinea pigs, so the portals have already been placed in the rooms, and their priority is the same priority associated to their room. This way, one can only move from a room to another if there are portals connecting them and the priority of the destiny room is lower than the current room's. The loser will be the player who has no valid move and thus, is doomed to receive no cake and possibly die in a fire.</p>
<h3>Input</h3>
<p>The input consists of several test cases.</p>
<p>The rst line of each test case will begin with two integers N, M denoting the number of rooms and the number of portal connections, 0 &lt; N ≤ 1000 and 0 ≤ M ≤ N (N − 1)/2. Rooms are numbered from 0 to N − 1, and their priority is the same as their number.</p>
<p>Then follows M lines describing the connections between two rooms. Each line contains two integers corresponding to rooms connected by portals.</p>
<p>The next line contains an integer K , 1 ≤ K &lt; N , denoting the number of test subjects. Two or more subjects may occupy the same room.</p>
<p>Next K lines contain the room numbers where the subjects have been alocated.</p>
<h3>Output</h3>
<p>For each test case, assuming both you and GLaDOS play perfectly and you are the first player to<br>make a move, print "I win" if you are victorious and "I lose" otherwise.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
9 14<br>0 1<br>0 2<br>0 3<br>1 2<br>2 3<br>1 4<br>2 5<br>5 3<br>4 5<br>4 3<br>5 6<br>6 7<br>7 8<br>8 6<br>3<br>3<br>5<br>8

<strong>Output:</strong>
I lose
</pre>