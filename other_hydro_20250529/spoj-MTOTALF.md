<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/MTOTALF/en/">English</a></td> 
<td width="50%"><a href="/problems/MTOTALF/vn/">Vietnamese</a></td> 
</tr></tbody></table>

<pre>Farmer John always wants his cows to have enough water and thus has
made a map of the N (1 &lt;= N &lt;= 700) water pipes on the farm that
connect the well to the barn. He was surprised to find a wild mess
of different size pipes connected in an apparently haphazard way.
He wants to calculate the flow through the pipes.

Two pipes connected in a row allow water flow that is the minimum
of the values of the two pipe's flow values. The example of a pipe
with flow capacity 5 connecting to a pipe of flow capacity 3 can
be reduced logically to a single pipe of flow capacity 3:

  +---5---+---3---+    -&gt;    +---3---+

Similarly, pipes in parallel let through water that is the sum of
their flow capacities:

    +---5---+
 ---+       +---    -&gt;    +---8---+
    +---3---+

Finally, a pipe that connects to nothing else can be removed; it
contributes no flow to the final overall capacity:

    +---5---+
 ---+               -&gt;    +---3---+
    +---3---+--

All the pipes in the many mazes of plumbing can be reduced using
these ideas into a single total flow capacity.

Given a map of the pipes, determine the flow capacity between the
well (A) and the barn (Z).

Consider this example where node names are labeled with letters:

                 +-----------6-----------+
        A+---3---+B                      +Z
                 +---3---+---5---+---4---+
                         C       D

Pipe BC and CD can be combined:

                 +-----------6-----------+
        A+---3---+B                      +Z
                 +-----3-----+-----4-----+
                             D

Then BD and DZ can be combined:

                 +-----------6-----------+
        A+---3---+B                      +Z
                 +-----------3-----------+

Then two legs of BZ can be combined:

                 B
        A+---3---+---9---+Z

Then AB and BZ can be combined to yield a net capacity of 3:

        A+---3---+Z

Write a program to read in a set of pipes described as two endpoints
and then calculate the net flow capacity from 'A' to 'Z'. All
networks in the test data can be reduced using the rules here.

Pipe i connects two different nodes a_i and b_i (a_i in range
'A-Za-z'; b_i in range 'A-Za-z') and has flow F_i (1 &lt;= F_i &lt;=
1,000). Note that lower- and upper-case node names are intended
to be treated as different.
</pre>

<br><c><h3>INPUT</h3></c>
<pre>* Line 1: A single integer: N

* Lines 2..N + 1: Line i+1 describes pipe i with two letters and an
        integer, all space-separated: a_i, b_i, and F_i

SAMPLE INPUT  

5
A B 3
B C 3
C D 5
D Z 4
B Z 6

</pre>
<c><h3>OUTPUT </h3></c>
<pre>* Line 1: A single integer that the maximum flow from the well ('A')
        to the barn ('Z')

SAMPLE OUTPUT  

3
</pre>