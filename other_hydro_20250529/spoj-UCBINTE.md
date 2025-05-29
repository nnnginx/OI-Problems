<p>The new semester at Hogwarts has just started, but something is not quite right —&nbsp;the staircases are not cooperating with the school administrators! Hogwarts has a single room of movable staircases connecting the N &nbsp;floors. There are M staircases in total, and no two staircases connect the same pair of floors (and, obviously, a staircase would not connect a &nbsp;floor to itself —&nbsp;these are smart magic staircases with dignity). The only way to manipulate the staircases is by pressing red and green buttons located on each floor. The floors are labeled in some manner by the integers 0 through N −&nbsp;1. Pressing the red button on &nbsp;floor i (0 ≤ i ≤ N −&nbsp;1) has the following effect on the staircases. Any staircase that is currently not connected to floor i does not move. Suppose a staircase connects floors i and j (j ≠&nbsp;i). After pressing the red button on floor i, it will instead connect &nbsp;floors i and j + 1 mod N —unless j + 1 mod N = i, in which case it will connect floors i and j +2 mod N = i+1 mod N instead. Pressing the green button is simply the inverse operation of pressing the red one on the same &nbsp;floor (or, equivalently, the same as pressing the red one N − 2 times).</p>
<p>While alone, the staircases got all messed up. The school adminstrators have presented a plan for how they would rather like the staircases to be placed.</p>
<p>You, a low-ranking house elf, have been given the task to fix this.</p>
<p>Find some sequence of at most 250 000 button presses that will change the staircase room from its current state to the desired state.</p>
<h3>Input</h3>
<p>There is a single test case. On the first line N and M are given (3 ≤ N ≤ 50, 0 ≤ M ≤ N(N −&nbsp;1)⁄2).</p>
<p>Then follow M lines with pairs of integers i, j (0 ≤ i, j ≤ N −&nbsp;1), describing the current state of the room of staircases. Each such line means that there is a staircase connecting &nbsp;floors i and j. After this follow another M lines with pairs of integers i, j, describing the desired state of the room of staircases.</p>
<h3>Output</h3>
<p>On the first line of output, write a single integer Q (0 ≤&nbsp;Q ≤ 250 000), the length of your sequence of button presses. Then print Q lines, each being either "R i" or "G i" for some i (0 ≤&nbsp;i ≤ N −&nbsp;1), meaning that the red or green button on floor i should be pressed.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5 4
0 1
0 3
1 2
2 4
0 2
0 4
2 3
2 4

<strong>Output:</strong>
2
R 0
G 2
</pre>
<pre><strong>Input:</strong>
3 3
0 1
0 2
1 2
0 1
1 2
0 2

<strong>Output:</strong>
0
</pre>