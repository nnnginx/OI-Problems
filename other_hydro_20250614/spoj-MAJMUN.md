<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/MAJMUN/en/">English</a></td>
<td width="50%"><a href="/problems/MAJMUN/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p>
</p><p>Coming home after a hard day at school, Ivica is ready to relax playing the computer game "Monkey &amp;banana". In the game, the monkey is located in a jungle, modeled as a coordinate plane.Every point with integer coordinates represents a tree. The monkey is initially located at tree (XM ,YM ) facing up i.e.towards the tree (XM ,YM +1).The monkey is controlled with the keys 0 to 7.When the key K is pressed,the monkey turns 45 degrees left K times and then jumps to the first tree he sees in his new direction.</p>
<p>The game lasts until the monkey jumps exactly N times.After that,the score is calculated from the distance between the monkey and the banana tree,which is located at coordinates (XB ,YB ).The lower the distance,the bigger the score. Ivica played one game and is now interested if he could have done better changing at most one key press. Write a program that determines the smallest possible ending (Euclidean) distance between the monkey and the banana tree (it is possible that the current score cannot be improved).</p>
<h3>Input</h3>
<p>The first line of input contains our integers XM ,YM ,XB and YB (0 XM ,YM ,XB ,YB 1 000 000),the initial coordinates of the monkey and the coordinates o the banana tree. The next line contains the integer N (1 ≤N ≤100 000),the number o jumps (key presses)in the game played.</p>
<p>The last line contains a string o N digits between 0 and 7,the keys that Ivica pressed.</p>
<h3>Output</h3>
<p>Output a single decimal number,the smallest achievable distance.Your output must be accurate to ±0.01.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
0 0 2 3
5
15102


<strong>Output:</strong>
0.000000
</pre>
<pre><strong>Input:</strong>
5 5 10 5
3
000


<strong>Output:</strong>
2.000000
</pre>
<pre><strong>Input:</strong>
0 0 10 10
9
700003000


<strong>Output:</strong>
1.414214
</pre>
<p> </p>