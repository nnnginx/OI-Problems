<p>Conflicts are everywhere in the world, from the young to the elderly, from families to countries. Conflicts cause quarrels, fights or even wars. How wonderful the world will be if all conflicts can be eliminated.</p>

<p>Edward contributes his lifetime to invent a 'Conflict Resolution Terminal' and he has finally succeeded. This magic item has the ability to eliminate all the conflicts. It works like this:</p>

<p>If any two people have conflict, they should simply put their hands into the 'Conflict Resolution Terminal' (which is simply a plastic tube). Then they play 'Rock, Paper and Scissors' in it. After they have decided what they will play, the tube should be opened and no one will have the chance to change. Finally, the winner have the right to rule and the loser should obey it. Conflict Eliminated!</p>

<p>But the game is not that fair, because people may be following some patterns when they play, and if the pattern is founded by others, the others will win definitely.</p>

<p>Alice and Bob always have conflicts with each other so they use the 'Conflict Resolution Terminal' a lot. Sadly for Bob, Alice found his pattern and can predict how Bob plays precisely. She is very kind that doesn't want to take advantage of that. So she tells Bob about it and they come up with a new way of eliminate the conflict:</p>

<p>They will play the 'Rock, Paper and Scissors' for <b>N</b> round. Bob will set up some restricts on Alice. But the restrict can only be in the form of <q>you must play the same (or different) on the <i>i</i>-th and <i>j</i>-th rounds</q>. If Alice loses in any round or break any of the rules she loses, otherwise she wins.</p>

<p>Will Alice have a chance to win?</p>

<h3>Input</h3>
<p>The first line contains an integer <b>T</b> (1 �� <b>T</b> �� 50), indicating the number of test cases.</p>

<p>Each test case contains several lines.
The first line contains two integers <b>N</b>, <b>M</b> (1 �� <b>N</b> �� 10000, 1 �� <b>M</b> �� 10000), representing how many round they will play and how many restricts are there for Alice.</p>

<p>The next line contains <b>N</b> integers <b>B</b><sub>1</sub>, <b>B</b><sub>2</sub>, ..., <b>B</b><sub><b>N</b></sub>, where <b>B</b><sub>i</sub> represents what item Bob will play in the <i>i</i>-th round. 1 represents Rock, 2 represents Paper, 3 represents Scissors.</p>

<p>The following <b>M</b> lines each contains three integers <b>A</b>, <b>B</b>, <b>K</b> (1 �� <b>A</b>,<b>B</b> �� <b>N</b>, <b>K</b>=0 or 1) represent a restrict for Alice. If <b>K</b> equals 0, Alice must play the same on <b>A</b>-th and <b>B</b>-th round. If <b>K</b> equals 1, she must play different items on <b>A</b>-th and <b>B</b>-th round.</p>

<h3>Output</h3>
<p>For each test case in the input, print one line: <tt>"Case #X: Y"</tt>, where <b>X</b> is the test case number (starting with 1) and <b>Y</b> is <tt>"yes"</tt> or <tt>"no"</tt> represents whether Alice has a chance to win.</p>

<h3>Example</h3>

<pre><b>Input:</b>
2
3 3
1 1 1
1 2 1
1 3 1
2 3 1
5 5
1 2 3 2 1
1 2 1
1 3 1
1 4 1
1 5 1
2 3 0

<b>Output:</b>
Case #1: no
Case #2: yes
</pre>