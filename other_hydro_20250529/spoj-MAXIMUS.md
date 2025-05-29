<p align="justify">Commodus has
discovered with your help that the traitor is Maximus. Commodus has
gathered N prestigious armies A1 A2 ... AN and asked you to lead them
to kill Maximus. A brave warrior like you must now act intelligently to
lead the armies to victory.</p>
<p align="justify">There are three countries which are considered here,
for simplicity lets name them C<sub>0</sub>, C<sub>1</sub>
and C<sub>2</sub>.
You have moved the armies to C<sub>0</sub> and you know that
Maximus is in C<sub>2</sub>.
You are wise enough to know that without all
your N armies you stand no chance against great Maximus. The problem is
that your armies are too egoistic in nature ( after all they were
organized by Commodus ). Only the biggest army can leave any country C<sub>y</sub>
(Army A<sub>x</sub> can leave C<sub>y</sub>, if there is no army A<sub>i</sub>
in C<sub>y</sub> with i &gt; x.). Also, the army A<sub>x</sub>
will go into C<sub>y</sub> only if it is the biggest army to get there,
i. e. there is no army A<sub>i</sub> in C<sub>y</sub> with i &gt; x.</p>
<p align="justify">There is another confusion here, all the
armies A<sub>m</sub> have been trained by a different
commander
and they march differently. Each army A<sub>m</sub> where m is either 1
or prime can only move
from C<sub>i</sub> to C<sub>(i+1)%3</sub>, while your armies A<sub>m</sub>
where m &gt; 1 is
composite will march only from C<sub>i</sub> to C<sub>(i+2)%3</sub>.
</p>
<p align="justify">Commodus is impatient and he is asking you to find
the
number of moves you need to reach Maximus. You are planning to reach
there with the shortest possible number of moves; tell your answer to
Commodus.</p>
<p align="justify">
Example for N = 2:<br>
The required number of steps would be 7<br>
initially<br>
C0 - A1, A2<br>
C1 -<br>
C2 -<br>
<br>
after step 1<br>
C0 - A1<br>
C1 - A2<br>
C2 -<br>
<br>
after step 2<br>
C0 - A1<br>
C1 - <br>
C2 - A2<br>
<br>
after step 3<br>
C0 - <br>
C1 - A1<br>
C2 - A2<br>
<br>
after step 4<br>
C0 - A2<br>
C1 - A1<br>
C2 - <br>
<br>
after step 5<br>
C0 - A2<br>
C1 - <br>
C2 - A1<br>
<br>
after step 6<br>
C0 - <br>
C1 - A2<br>
C2 - A1<br>
<br>
after step 7<br>
C0 - <br>
C1 - <br>
C2 - A1, A2<br>
</p>
<h3>Input</h3>
<p>The input will consist of at most 100 test cases. Each test case consists of a number N (the number of armies, 1 �� N �� 5000).
The last test case is followed by a line containing 0.
</p>
<h3>Output</h3>
<p>For each number N, you have to output the number of moves needed to move the
armies to C<sub>2</sub> with the minimum number of steps.
</p>
<h3>Example</h3>

<pre><b>Input:</b>
1
2
3
4
100
0

<b>Output:</b>
2
7
21
49
1299510268586153115889930564780511199231
</pre>