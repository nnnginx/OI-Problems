<p>
Hey, ACRush and Jelly are playing a game ! Let take a look at its rule: </p>
<p>You are given a tree. Two players take turns cutting edges on a tree. Some nodes is on the "ground".
When a player cuts an edge, all the edges that are no longer connected to the ground disappear.
The player who can not take a move loses.
</p>
<p>ACRush plays first. Both of them are very good players. If you know state of the tree they are playing with, can you guess who will win?</p>

<img src="/content/thanhvy:green_fig.png">
     Node 4 is on the ground.
<h3>Input</h3>
<p>    Input consists of multiple test-cases. The first line contains one integer <i>t</i> - number of cases (0 &lt; <i>t</i> &lt;= 20).
    For each case, the input format is following.

    The first line contains one integer <i>N</i> (1 &lt;= <i>N</i> &lt;= 100000).
    The next line <i>N</i> integers s[i] (1 or 0).
    If s[i] is 1, the <i>i</i>-th node is on the ground.
    If s[i] is 0, the <i>i</i>-th node is not on the ground.

    Each line of the following <i>N</i> - 1 lines contains two integers u, v.
    They denote there is an edge between node u and node v (1 &lt;= u,v &lt;= N).<br>
There is no blank line after each case.

</p><h3>Output</h3>
<p>
    For each case, output who will win the game. If ACRush wins, output <i>1</i>; otherwise, output <i>0</i> (Jelly wins).<br>
There is no blank line after each case.

</p><h3>Example</h3>

<pre><b>Input:</b>
1
4
0 0 0 1
1 2
2 3
2 4

<b>Output:</b>
1
</pre>