<p>You are given the scores of several players in a competition. Your task is to create a ranklist of the
players, sorted in decreasing order by score.</p>
<p>
Unfortunately, the data structure used for the list of players supports only one operation, which
moves a player from position i to position j without changing the relative order of other players. If
i &gt; j, the positions of players at positions between j and i − 1 increase by 1, otherwise if i &lt; j the
positions of players at positions between i + 1 and j decrease by 1.</p>
<p>
This operation takes i steps to locate the player to be moved, and j steps to locate the position
where he or she is moved to, so the overall cost of moving a player from position i to position j is
i + j. Here, positions are numbered starting with 1.</p>
<p>
Determine a sequence of moves to create the ranklist such that the sum of the costs of the moves is
minimized.
</p>
<h3>Input</h3>
<p>The input consists of <b>exactly 10</b> test cases. The first line of each test case contains n (2 ≤ n ≤ 1000),
the number of players. Each of the following n lines contains one non-negative integer s<sub>i</sub> (0 ≤ s<sub>i</sub> ≤ 1000000), the scores of the players in the current order. You may assume that all scores are distinct.
</p>
<h3>Output</h3>
<p>For each test case, print in one line the number of moves used to create the ranklist. The following lines should specify the moves in the
order in which they are applied. Each move should be described by a line containing two integers i
and j, which means that the player at position i is moved to position j. The numbers i and j must be
separated by a single space.
</p>
<h3>Example</h3>
<i>here only one test case</i>
<pre><b>Input:</b>
5
20
30
5
15
10

<b>Output:</b>
2
2 1
3 5
</pre>