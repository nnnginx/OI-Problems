<p>A magic star consists of all the numbers from <em>1</em> to <em>12</em> arranged in the shape of a hexagram:</p>
<p style="text-align: center;"><img src="../../../content/ak15:magicstar.png" alt="example image"></p>
<p>The magic comes from the fact that in each line of <em>4</em> numbers, the sum of the numbers is <em>26</em>. In the example given above, the six lines consist of the following numbers:</p>
<ul>
<li><em>1 + 4 + 10 + 11</em></li>
<li><em>11 + 5 + 3 + 7</em></li>
<li><em>7 + 6 + 12 + 1</em></li>
<li><em>2 + 10 + 5 + 9</em></li>
<li><em>9 + 3 + 6 + 8</em></li>
<li><em>8 + 12 + 4 + 2</em></li>
</ul>
<p>There are several possible ways to arrange the numbers to get a magic star. Given a partially labelled star, your task is to extend the solution such that a magic star is formed.</p>
<h3>Input</h3>
<p>The input consists of a visualization of the star; the unlabelled fields of the star will be represented by an 'x' character, and labelled fields will contain a letter between 'A' and 'L', where the <em>i</em>-th letter in the alphabet represents number <em>i</em>. The character '.' is used to align the fields of the star in the shape of a hexagram. You may assume that each input will use the same alignment of the fields as the one in the sample input.</p>
<h3>Output</h3>
<p>Print the lexicographically smallest extension of the given partial solution which is a magic star (lexicographically smallest means that the concatenation of the rows should result in a string which is lexicographically smaller than other potential solutions). You may assume that there is always a solution for the given input.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
....x....
.A.I.D.x.
..x...x..
.x.x.x.x.
....x....

<strong>Output:</strong>
....F....
.A.I.D.L.
..H...E..
.C.J.B.K.
....G....
</pre>