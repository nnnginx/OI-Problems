<p>Ada the Ladybug has sequence of different vegetables (for simplicity represented by numbers). She has a few interesting questions of following form: Choose some continuous subsequence of vegetables, then assign each kind of vegetable a distinct positive number. She wants to assign them in a way that the sum (of assigned numbers) over all vegetables will be as low as possible.</p>
<h3>Input</h3>
<p>The first line contains two integers <strong>1 ¡Ü N, Q ¡Ü     2*10<sup>5</sup></strong>, the number of vegetables and number of questions.</p>
<p>Next line contains <strong> N </strong> integers <strong>1 ¡Ü A<sub>i</sub> ¡Ü     10<sup>9</sup></strong>, the kinds of vegetables.</p>
<p>Next <strong>Q</strong> lines contains two integers <strong>1 ¡Ü I ¡Ü J ¡Ü N </strong>, the left and right indices of Ada's questions.</p>
<h3>Output</h3>
<p>For each question answer the minimal possible sum.</p>
<h3>Example Input 1</h3>
<pre>10 5
1 1 3 2 4 1 3 1 1 4
1 3
1 10
5 10
3 5
5 8
</pre>
<h3>Example Output 1</h3>
<pre>4
19
10
6
7
</pre>
<h3>Example IO explanation</h3>
<p>Assign 1 to 1 and 2 to 3</p>
<p>Assign 1 to 1, 2 to 4, 3 to 3 and 4 to 2 (swapping 4 and 3 would work too)</p>
<p>Assign 1 to 1 and 2 to 4 and 3 to 3</p>
<p>Assign 1 to 4, 2 to 3 and 3 to 4 (but any permutation would do)</p>
<p>Assign 1 to 1 and 2 to 4 and 3 to 3</p>