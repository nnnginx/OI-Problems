<p>Aman, Gitanshu and Vishal have recently been selected as admins of DCE Coders. Kapish is pretty happy with the selection, but he wants to make sure that the new admins understand the importance of team-work if they are to take DCE Coders forward in the coming year. Keeping this in mind, he challenges the 3 of them to a game.</p>
<p>Kapish takes all 3 of them to a long narrow corridor, and gives each of them separate start and end coordinates. The task is simple: All of them have to go from their start coordinates to their respective end coordinates simultaneously (i.e. using the same number of moves). However, they can only move in some discrete steps, which are also given by Kapish. He provides one array (of size ¡®N¡¯) of acceptable jumps to each of the 3.&nbsp; The challenge is that in one move, all 3 of them have to agree upon 1 common index (from 0 to N-1) and then they would add the value corresponding to that index from their respective arrays to get their new coordinates.</p>
<p>Now Pushap, who likes challenges (such as jumping off moving trains!!), further complicates the problem. If the index selected in the previous move is odd, then it must be even for the current move, and vice versa. They can choose any index for the first move.</p>
<p>The 3 new admins are required to find the minimum number of moves in which all 3 of them can simultaneously reach their destinations. Can you help them?</p>
<p>Note 1: You can assume the corridor is 1 dimensional and infinite.</p>
<p>Note 2: It is possible for more than 1 person to be on the same coordinate at the same time.</p>
<h3>Input</h3>
<p>First line of input contains T the number of test cases</p>
<p>First line of each test case contains 3 separated integers, A1, G1 and V1, the initial coordinates for the 3.</p>
<p>Next line contains 3 space separated integers, A2, G2 and V2, the final coordinates for the 3.</p>
<p>Next line contains a single integer, N.</p>
<p>Next 3 lines contain N space separated integers each, denoting arrays A, G and V of acceptable jumps for the 3.</p>
<h3>Output</h3>
<p>Output a single integer (in a separate line) per test case, containing the minimum number of moves.</p>
<p>If it is not possible for them to reach their destinations simultaneously, output -1.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p>1</p><p>1 2 3</p><p>2 3 5</p><p>2</p><p>1 3</p><p>1 2</p><p>2 1</p>
<strong>Output:</strong>
1
</pre>
<pre><p><strong>Explanation:</strong></p><p>The 3 of them can choose index 0 in the first move to reach their destinations.</p><p>&nbsp;</p><p><strong>Constraints:</strong></p><p>1 &lt;= T &lt;= 5</p><p>-50 &lt;= A1, A2, G1, G2, V1, V2 &lt;= 50</p><p>1 &lt;= N &lt;= 20</p><p>-10 &lt;= A[i], G[i], V[i] &lt;= 10</p></pre>