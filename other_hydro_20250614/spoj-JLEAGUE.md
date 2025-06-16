<p>Thirty five years ago, a group of super heroes was chosen to form the Justice League, whose
purpose was to protect the planet Earth from the villains. After all those years helping mankind,
its members are retiring and now it is time to choose the new members of the Justice League.

</p><p></p><p>
In order to keep their secret identity, let¡¯s say, secret, super heroes usually use an integer number
to identify themselves. There are H super heroes on Earth, identified with the integers from 1
to H. With a brief look at the newspapers anyone can find out if two super heroes have already
worked together in a mission. If this happened, we say that the two heroes have a relationship.

</p><p></p><p>
There must be only <i>one</i> Justice League in the world, which could be formed by any number of
super heroes (even only one). Moreover, for any two heroes in the new league, they <i>must</i> have
a <i>relationship</i>.

</p><p></p><p>
Besides, consider the set of the heroes not chosen to take part in the Justice League. For any
two heroes on that set, they <i>must not</i> have a relationship. This prevents the formation of
unofficial justice leagues.

</p><p></p><p>
You work for an agency in charge of creating the new Justice League. The agency doesn¡¯t know
if it is possible to create the League with the restrictions given, and asked for your programming
skills. Given a set of super heroes and their relationships, determine if it is possible to select
any subset to form the Justice League, according to the given restrictions.

</p><h3>Input</h3>
<p>The input is composed of several test cases. The first line of each test case contains two integers
separated by a single space, H (2 &lt;= H &lt;= 5¡Á10<sup>4</sup>) and R (1 &lt;= R &lt;= 10<sup>5</sup>), indicating, respectively,
the number of heroes and the number of relationships. Each of the following R lines contains
two integers separated by a single space, A and B (1 &lt;= A &lt; B &lt;= H), indicating that super
hero A has a relationship with super hero B. Note that if A has a relationship with B, B also
has a relationship with A. A relationship is never informed twice on a test case.

</p><p></p><p>
The end of input is indicated by H = R = 0.

</p><h3>Output</h3>
<p>For each test case in the input print a single line, containing the uppercase letter ¡°Y¡± if it
is possible to select a subset of heroes to form the Justice League according to the given
restrictions, or the uppercase letter ¡°N¡± otherwise.

</p><h3>Example</h3>

<pre><b>Input:</b>
5 5
1 2
2 3
1 3
1 4
3 5
9 8
1 2
2 3
3 4
4 5
5 6
6 7
7 8
8 9
4 3
1 2
2 3
3 4
0 0

<b>Output:</b>
Y
N
Y
</pre>