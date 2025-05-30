<p>

Flavius Josephus and 40 fellow rebels were trapped by the Romans.
His companions preferred suicide to surrender, so they decided to form a circle and to kill every third person and to proceed around the circle until no one was left.
Josephus was not excited by the idea of killing himself, so he calculated the position to be the last man standing (and then he did not commit suicide since nobody could watch).

</p><p>

We will consider a variant of this "game" where every second person leaves.
And of course there will be more than 41 persons, for we now have computers.
You have to calculate the safe position.
Be careful because we might apply your program to calculate the winner of this contest!

</p><h3>Input Specification</h3><p>

The input contains several test cases.
Each specifies a number <code>n</code>, denoting the number of persons participating in the game.
To make things more difficult, it always has the format <tt>"</tt><code>xy</code><tt>e</tt><code>z</code><tt>"</tt> with the following semantics: when <code>n</code> is written down in decimal notation, its first digit is <code>x</code>, its second digit is <code>y</code>, and then follow <code>z</code> zeros.
Whereas <code>0&lt;=x,y&lt;=9</code>, the number of zeros is <code>0&lt;=z&lt;=6</code>.
You may assume that <code>n&gt;0</code>.
The last test case is followed by the string <tt>00e0</tt>.


</p><h3>Output Specification</h3><p>

For each test case generate a line containing the position of the person who survives.
Assume that the participants have serial numbers from <code>1</code> to <code>n</code> and that the counting starts with person 1, i.e., the first person leaving is the one with number 2.
For example, if there are 5 persons in the circle, counting proceeds as <code>2, 4, 1, 5</code> and person <code>3</code> is staying alive.

</p><h3>Sample Input</h3><p>

</p><pre>05e0
01e1
42e0
66e6
00e0
</pre>

<h3>Sample Output</h3><p>

</p><pre>3
5
21
64891137
</pre>