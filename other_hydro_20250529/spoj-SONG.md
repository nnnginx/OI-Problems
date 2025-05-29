<p>Every year, the continent of Cacophonea organises the Cacophonean Song Contest, for which each
of its nations presents an act by a national singer or group. Each Cacophonean inhabitant may
televote for any act which is not from his nation, so a nation can never vote for its own act. In
the end, each of the <b>s</b> Cacophonean nations will award points to <b>r</b> acts. The act which received
most votes from a certain nation will get <b>r</b> points from this nation, the act with the second largest
amount of votes will get <b>r</b> - 1 points, etc., so the act with the <b>r</b>th largest amount of votes gets 1
point and less popular acts get no points from the voting nation. The final ranking of the song
contest will then be decided by the total amount of points each nation received.
</p><p>Music producer Dustin has been eagerly following the Cacophonean Song Contest for many
years. Lately, he has observed that in certain nations, televotes are politically rather than artistically motivated:
</p><p>(1) Politically voting nations prefer acts from neighbouring nations. More specifically, the Euclidean distance between their capital and another nation's capital is their popularity measure, irregardless of the artistic quality of the corresponding act. Hence, the nation with the
closest capital will get most votes and the nation with the farthest capital will receive the
least votes, which could yield no points at all if <b>r</b> &lt; <b>s</b> - 1. It will never occur that two or
more capitals will have the same distance to a certain capital.
</p><p>(2) Nations that vote quality-motivated will, as the name suggests, award points to nations
according to an indisputable act ranking based on each act's artistic quality. In this ranking,
there will be no ties so each nation has its own unique rank.
</p><p>However, Dustin has heard he can influence the voting behaviour of other nations: an artist can
find favour of politically voting nations by giving them special attention during his act (e.g. by
singing parts in their local dialects, waving their flags, etcetera). The more a politically voting
nation will receive such attention in an act, the higher it will rank it. Of course this will be at the
cost of the original act and might result in terribly campy results. Therefore, nations that vote
according to artistic quality will punish such behaviour.
</p><p>More specifically, Dustin can divide an act into exactly <b>s</b> - 1 parts. Originally, all parts are
dedicated to the nation of the performer (i.e. they reflect his original artistic ideas), but this can
be changed:
</p><p>(1) For each part in the act that will be dedicated to a certain politically voting nation, that
nation will rank the performer's nation one place higher (unless the performer's nation is
already ranked first). As each nation has a unique ranking position, the nation that originally
was at that higher rank will then be ranked one place lower.
</p><p>(2) Quality-motivated voting nations do not like these soft-soaping attempts at all. Therefore,
for each part in the act that will be dedicated to a nation which is not the original performer's
nation, quality-motivated nations will rank the original performer's nation one place lower
(unless the performer's nation is already ranked lowest).
</p><p>Only the fact that a certain amount of parts is dedicated to a certain nation will influence voting
behaviour: the exact part dedication sequence in the total act is not of interest here.
</p><p>Dustin wants to use this knowledge (which no other Cacophonean producer has) to produce a
smashing act, yielding as much points in the overall results as possible. You are asked to determine
what the largest possible overall point score is he can obtain for an act, when he optimally exploits
the described act-changing practices.</p>
<h3>Input</h3>
<p>The first line of input consists of the integer number <b>n</b>, the number of test cases;
</p><p>Then, for each test case:
</p><p>A line with an integer number <b>s</b> (1 &lt; <b>s</b> &lt;= 100), indicating the number of participating
nations in the song contest;
</p><p>Then, for each nation:
</p><p>(1) A line containing:
</p><p>(1.1) A string <b>c</b> (not containing any spaces) with the nation's name, followed by a
space. Within a test case, there will not be multiple nations sharing the same
name;
</p><p>(1.2) A character indicating the nation's voting behaviour: <i>q</i> if the voting behaviour
is quality-motivated and <i>p</i> if the behaviour is politically motivated.
</p><p>(2) A line containing:
</p><p>(2.1) The location of the nation's capital, expressed in an (x, y) integer coordinate
(-10000 &lt;= x &lt;= 10000, -10000 &lt;= y &lt;= 10000). x and y are separated by a
space. Furthermore, y is followed by a space;
</p><p>(2.2) The actual artistic quality rank <b>q</b> of the nation's act. This is a unique number
in the range 1...<b>s</b>.
</p><p>After description of each nation:
</p><p>A line with an integer number <b>r</b> (0 &lt; <b>r</b> &lt;= <b>s</b> - 1), indicating to how many nations each
nation will attribute points;
</p><p>A line with the name of the nation for which Dustin should produce a song, achieving
as much points as possible.</p>
<h3>Output</h3>
<p>For each test case, the output contains a single line with a single integer number: the maximal amount of points an act can obtain in the overall final score, if act-changing practices were performed in an optimal way.</p>

<h3>Example</h3>
<pre><b>Input:</b>
2
3
Aulatrias q
0 0 1
Binen q
5 0 2
Cahin q
0 -4 3
2
Cahin
3
Aulatrias p
0 0 1
Binen p
5 0 2
Cahin p
0 -4 3
2
Binen

<b>Output:</b>
2
4
</pre>