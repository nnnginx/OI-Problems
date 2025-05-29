<p>
In the time of Louis XIII and his powerful minister cardinal Richelieu in the Full Barrel Inn
<i> n</i> musketeers had consumed their meal and were drinking wine. Wine had not run short and
therefore the musketeers were eager to quarrel, a drunken brawl broke out, in which each musketeer insulted all the
others.
</p>

<p>
A duel was inevitable. But who should fight who and in what order? They
decided (for the first time since the brawl they had done something
together) that they would stay in a circle and draw lots in order. A
drawn musketeer fought against his neighbor to the right. A looser
"quit the game" and to be more precise his corpse was taken away by
servants. The next musketeer who stood beside the looser became the
neighbor of a winner.&nbsp;
</p>

<p>After years, when historians read memories of the winner they
realized that a final result depended in a crucial extent on the order
of duels. They noticed that a fence practice had indicated, who
against who could win a
duel. It appeared that (in mathematical language) the relation "<b>A</b> wins
<b>B</b>" was not transitive! It could happen that the musketeer <b> A</b> fought better than
<b>B</b>, <b> B</b> better than <b> C</b> and <b> C</b> better than <b>A</b>. Of course, among three of them the first duel influenced the final result. If
<b> A </b> and <b> B</b> fight as the first, <b> C</b> wins eventually. But if <b> B</b> and
<b> C</b> fight as the first, <b> A</b> wins finally. Historians
fascinated by their discovery decided to verify which musketeers could
survive. The fate of France and the whole civilized Europe indeed
depended on that!
</p>

<h3>Task</h3>
<p>
<i>
N</i> persons with consecutive numbers from <i> 1</i> to <i> n</i> stay in a circle. They fight
<i> n-1</i> duels. In the first round one of these persons (e.g. with the number
<i> i</i>) fights against its neighbor to the right, i.e. against the person numbered <i> i+1</i> (or, if
<i>i=n</i>, against the person numbered <i>1</i>).  A looser quits the game, and
the circle is tighten so that the next person in order becomes a winner's neighbor. We are given the
table with possible duels results, in the form of a matrix. If <b>A</b><i>i,j</i> = 1
then the person with the number
<i> i</i> always wins with the person <i>j</i>. If <b>A</b><i>i,j</i> = 0 the person
<i>i</i> looses with <i>j</i>. We can say that the person<i> k</i> may win the game if there exists such a series of
<i>n-1</i> drawings, that <i>k</i>
wins the final duel.<br>
Write a program which:
</p>
<ul>
  <li>reads matrix <b> A</b> from the standard input,
  </li><li>computes numbers of persons, who may win the game,
  </li><li>writes them into the standard output.
</li></ul>

<h3>Input</h3>
<p>
The number of test cases t is in the first line of input, then t test cases follow separated by an empty line.
In the first line of each test case integer <i>n</i> which satisfies the inequality
<i> 3&lt;=n&lt;=100</i> is written. In each of the following <i> n</i> lines appears one word
consisting of
<i> n</i> digits 0 or 1. A digit on <i>j</i>-th position in<i> i</i>-th line denote <b>A</b><i>i,j.</i> Of course <b>A</b><i>i,j </i>= 1 - <b>A</b><i>j,i</i>, for <i> i&lt;&gt;j</i>. We assume that
<b>A</b><i>i,i </i>= 1, for each <i>i</i>.&nbsp;
</p>

<h3>Output</h3>
<p>
For each test case in the first line there should be written <i> m</i> - the
number of persons, who may
win the game. In the following <i> m</i> lines numbers of these persons should be written in  ascending order, one number in each line.
</p>

<h3>Example</h3>
<pre><b>Sample input:</b>
1
7
1111101
0101100
0111111
0001101
0000101
1101111
0100001

<b>Sample output:</b>
3
1
3
6
</pre>

<p>
The order of duels: 1-2, 1-3, 5-6, 7-1, 4-6, 6-1 gives a final victory to the person numbered 6. You can also check that only two persons more (1 and 3) may win the game.

</p>