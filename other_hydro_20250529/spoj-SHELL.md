<p>Your program is to play the traditional "shell" game (<a title="here" href="http://en.wikipedia.org/wiki/Shell_game" target="_blank">http://en.wikipedia.org/wiki/Shell_game</a>). The game is played as follows:</p>
<p>There is a person called an operator; he/she has 3 identical, non-transparent hollow objects - shells, and a metal ball, which he/she places under one of these objects. Then, the operator quickly swaps pairs of shells several times<span class="AM">; if shells at positions A and B are swapped, and the ball is unde</span>r the shell at position A, it moves under the shell at position B. In the end, you have to guess which shell the ball is under.</p>
<p>The shells are identical, and positions mean immediate position that you see (left will always denote the leftmost shell, not the shell that was leftmost in the beginning).</p>
<p>Input</p>
<p>The first line of input contains one string - "left", "center" or "right", denoting the position of the shell the ball is under in the beginning. The second line contains an integer N&lt;=10, denoting the number of swaps. N lines follow, all of them contain 2 strings - positions of 2 shells which are swapped.</p>
<p>Output</p>
<p>Output position of the shell the ball is under after all swaps are performed.</p>
<p>Warning</p>
<p>Testing simulates the exact progress of an actual game! There are 10 testcases<span class="AM">; in the last one only, N=10</span>. You're likely to get a WA on this last test case, even if your program seems correct. Remember, it's like an actual game!</p>
<p>Example</p>
<pre><strong>Input:</strong>
<br>left<br>2<br>left right<br>right center<br><strong><br>Output:</strong><br><br>center
<br>Explanation:<br>in the beginning, the ball is under the left shell<br>after swap 1, it's under the right shell<br>after swap 2, it's under the center shell<br></pre>