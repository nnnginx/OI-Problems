<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/PERIODNI/en/">English</a></td>
<td width="50%"><a href="/problems/PERIODNI/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p> </p>
<p>Luka is bored in chemistry class so he is staring at a large periodic table of chemical elements hanging from a wall above the blackboard. To kill time, Luka decided to make his own table completely different from the one in the classroom.</p>
<p>His table consists of N columns, each with some height, aligned at the bottom (see example below). After he draws the table he needs to fill it with elements. He first decided to enter the noble gases of which there are K. Luka must put them in the table so that no two noble gases are close to each other.</p>
<p>Two squares in the table are close to each other if they are in the same column or row, and all squares between them exist. In the example below, the 'a' squares are not close, but the 'b' squares are.</p>
<p><img src="./23826/file/aRn8L5O2.png" alt="" width="200" height="160"></p>
<p>Write a program that, given N, K and the heights of the N columns, calculates the total number of ways for Luka to place the noble gases into the table. This number can be large, so output it modulo 1 000 000 007.</p>
<h3>Input</h3>
<p>The first line contains the integers N and K separated by a space (1 ¡Ü N ¡Ü 500, 1 ¡Ü K ¡Ü 500), the number of columns in Luka's table and the number of noble gases.</p>
<p>The next line contains N positive integers, separated by spaces. These are heights of the columns from left to right. The heights will be at most 1 000 000.</p>
<h3>Output</h3>
<p>Output the number of ways for Luka to fill his table with noble gases, modulo 1 000 000 007.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5 2
2 3 1 2 4

<strong>Output:</strong>
43
</pre>
<p></p>