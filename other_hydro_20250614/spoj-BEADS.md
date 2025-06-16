<p>Once upon a time there was a famous actress. As you may expect, she played
mostly Antique Comedies most of all. All the people loved her. But she was not
interested in the crowds. Her big hobby were beads of any kind. Many bead
makers were working for her and they manufactured new necklaces and
bracelets every day. One day she called her main <i>Inspector of Bead
Makers</i> (<i>IBM</i>) and told him she wanted a very long and special
necklace.

</p><p>The necklace should be made of glass beads of different sizes connected
to each other but without any thread running through the beads, so that
means the beads can be disconnected at any point. The actress chose the
succession of beads she wants to have and the IBM promised to make the
necklace. But then he realized a problem. The joint between two neighbouring
beads is not very robust so it is possible that the necklace will get torn
by its own weight. The situation becomes even worse when the necklace is
disjoined. Moreover, the point of disconnection is very important. If there
are small beads at the beginning, the possibility of tearing is much higher
than if there were large beads. IBM wants to test the robustness of a
necklace so he needs a program that will be able to determine the worst
possible point of disjoining the beads.

</p><p>The description of the necklace is a string <var>A =
a<sub>1</sub>a<sub>2</sub> ... a<sub>m</sub></var>
specifying sizes of the particular beads, where the last character
<var>a<sub>m</sub></var> is considered to precede character
<var>a<sub>1</sub></var> in circular fashion. 

</p><p>The disjoint point <var>i</var> is said to be worse than the disjoint
point <var>j</var> if and only if the string
<var>a<sub>i</sub>a<sub>i+1</sub> ... a<sub>n</sub>a<sub>1</sub> ...
a<sub>i-1</sub></var> is lexicografically smaller than the string
<var>a<sub>j</sub>a<sub>j+1</sub> ... a<sub>n</sub>a<sub>1</sub> ...
a<sub>j-1</sub></var>.
String <var>a<sub>1</sub>a<sub>2</sub> ... a<sub>n</sub></var> is
lexicografically smaller than the string
<var>b<sub>1</sub>b<sub>2</sub> ... b<sub>n</sub></var> if and only if there
exists an integer <var>i, i &lt;= n</var>, so that
<var>a<sub>j</sub>=b<sub>j</sub></var>, for each <var>j, 1 &lt;= j &lt;
i</var> and <var>a<sub>i</sub> &lt; b<sub>i</sub></var>.


</p><h3>Input</h3>

<p>The input consists of <var>N</var> cases. The first line of the input
contains only positive integer <var>N</var>. Then follow the cases. 
Each case consists of exactly one line containing necklace description.
Maximal length of each description is 10000 characters. 
Each bead is represented by a lower-case character of 
the english alphabet (a--z), where <var>a &lt; b   ...   z</var>.


</p><h3>Output</h3>

<p>For each case, print exactly one line containing
only one integer -- number of the
bead which is the first at the worst possible disjoining, i.e. such
<var>i</var>, that the string <var>A[i]</var> is lexicographically smallest
among all the <var>n</var> possible disjoinings of a necklace. If there are
more than one solution, print the one with the lowest <var>i</var>.


</p><h3>Example</h3>
<pre>Sample input:

4
helloworld
amandamanda
dontcallmebfu
aaabaaa

Sample output:

10
11
6
5
</pre>