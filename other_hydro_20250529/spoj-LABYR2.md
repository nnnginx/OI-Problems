<p>Fred is a robotic mouse built by a group of students of artificial intelligence. Fred can move around in the labyrinth shown in the picture below. Whenever Fred comes to a place marked by a number, he has to choose one of the possible directions. Behavior of the mouse should look chaotic and complex enough so that it will impress students' supervisor.</p>
<pre>+--------4
|        |
|  8--9  |
|  |  |  |
2--7--0  |
|  |     |
1  6-----+
</pre>
<p>Numbered places in the labyrinth are called nodes. Fred has one integer X stored in its memory and can perform some calculations. In each node (except node 1) he chooses a direction according to X, decreases X by 1 and goes to the chosen node. The direction is chosen according to this rules:</p>
<pre>Node 2: Compute X mod 3.
        If the result is 0, go to 7
                         1, go to 1
                         2, go to 4.

Node 4: Let Y be X written backwards (in decimal system).
        If Y&gt;X then go to 6 otherwise go to 2.

Node 6: Compute the number of digits of X (in decimal system).
        If the result is even then go to 4 otherwise go to 7.

Node 7: Compute (X*X) mod 7.
        If the result is 0 go to 2
                         1 go to 6
                         2 go to 8
                         4 go to 0.

Node 8: Compute X mod 5.
        If the result is 2 or 3 then go to 7 otherwise go to 9.

Node 9: If you have come from 8 then go to 0.
        If you have come from 0 then go to 8.

Node 0: Let Y be the third least significant digit of X in decimal system
        (if X&lt;100 then Y=0). If Y&lt;=7 then go to 7 otherwise go to 9. 
</pre>
<p>At the beginning of each experiment, the experimenter puts the mouse in the node 0 and initializes value X by voice. After that, the mouse starts to move. The mouse displays current value of X on its digital display. The experiment finishes when the mouse enters the node 1, the result of the experiment is the number displayed. If the value of X decreases to zero, the experiment fails and its result is -1.</p>
<h3>Input file description</h3>
<p>The input file contains several initial values of X(less than two-million) as they were told by the experimenter.</p>
<h3>Output file description</h3>
<p>For each value of X in the input file write to a separate line of the output file the result of the corresponding experiment (see example output).</p>
<h3>Example</h3>
<pre><strong>Input file:</strong>
thirteen
fourteen
one-thousand
one-million-three-hundred-and-twenty-five-thousand-nine-hundred-and-seventy-nine

<strong>Output file:</strong>
-1
9
789
1325784
</pre>
<p><strong>Note</strong>: New test cases were added. Thanks to <a href="http://www.spoj.com/users/gerrob"> Robert Gerbicz</a> and <a href="http://www.spoj.com/users/triplem"> Stephen Merriman</a>'s discussion in the forum.</p>