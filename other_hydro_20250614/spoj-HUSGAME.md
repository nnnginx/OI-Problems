<p>Once our hero Huseyn invited Ziya the <span style="text-decoration: line-through;">ProGrammer</span> ProGamer to play his new game with him. Ziya has a great prestige in the gamers area, so he must win the game or ignore the invitation to save his reputation. The rules of the game are not difficult:</p>
<ul>
<li>Initially, there are <strong>N</strong> stones on the table. Huseyn will start the game and they will play alternatively.</li>
<li>Each turn consisting of replacing the number of stones <strong>n</strong> on the table with <strong>n-1 or [(n+1)/2]</strong>. Here <strong>[]</strong> is floor function.</li>
<li>The player who makes <strong>1 </strong>stone remain wins.</li>
</ul>
<p>As Ziya is busy with playing games (you know, he can't pause online games :P) you need to make an honest decision for him.</p>
<h3>Input</h3>
<p>There will be multiple test cases. The first line of the input consisting of the number of the test cases - <strong>T (1 ¡Ü T ¡Ü 10000)</strong>. For each test case, there will be only one line donating single integer <strong>- N (1 ¡Ü N ¡Ü 10<sup>18</sup>)</strong>.</p>
<h3>Output</h3>
<p>For each test case, print "ZiYES" if Ziya can win the game without matter of the Huseyn's moves, "HuseyNO" otherwise.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3<br>1<br>2<br>3<br><strong>Output:</strong>
HuseyNO<br>HuseyNO<br>ZiYES <br></pre>