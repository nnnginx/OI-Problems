<p>In a far away country there is a wide river, N villages on the left and N villages on the right side of this river (denoted by 1..N on each side). There are also M small ships, each of them connecting one village from the left and one village from the right side (in both ways).</p>
<p>You are to organize a film festival in four of these villages: two from the left and two from the right side. Each two of these four villages must be connected by a ship (directly) if they belong to opposite sides of the river.</p>
<p>Help yourself to choose these four villages and first find out; in how many ways can you choose them?</p>
<h3>Input</h3>
<p>In the first line there are integers N ¡Ü 1000 and M ¡Ü N<sup>2</sup>.</p>
<p>In the next M lines there are two integers from the interval [1, N] representing the village from the left and the village from the right side connected by this ship.</p>
<h3>Output</h3>
<p>Print the required number of ways to choose villages for the festival.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3 5<br>1 1<br>1 2<br>1 3<br>2 2<br>2 3<br>
<strong>Output:</strong>
1<br><br>(the only possibility is to choose the villages 1, 2 from the left and 2, 3 from the right side)</pre>