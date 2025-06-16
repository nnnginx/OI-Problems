<p>As you might know, Ada the Ladybug is a farmer. She needs to choose some species of vegetables. Each vegetable disposes with four important attributes. We say that a vegetable is worse than another vegetable, if all of its four attributes are greater.</p>
<p>She wants to eliminate the list of vegetables, so only vegetables, which are not worse than any other vegetables remains.</p>
<h3>Input</h3>
<p>The first line contains integer <strong>1 ¡Ü N ¡Ü 2*10<sup>5</sup></strong></p>
<p>Each of the next <strong>N</strong> lines contains four integers <strong>1 ¡Ü X, Y, Z, W     ¡Ü N</strong>. It is guaranteed, that all <strong>X</strong> attributes are distinct for all vegetables. The same is true for <strong>Y, Z </strong>and<strong> W</strong> (so in fact, there are four permutations of numbers from <strong>1</strong> to <strong>N</strong>).</p>
<h3>Output</h3>
<p>Print the number of vegetables, which are not worse than any other vegetable.</p>
<h3>Example Input 1</h3>
<pre>3
1 1 1 1
2 2 2 2
3 3 3 3
</pre>
<h3>Example Output 1</h3>
<pre>1
</pre>
<h3>Example Input 2</h3>
<pre>10
8 9 9 2
3 7 2 4
5 5 10 10
9 3 5 9
4 6 8 6
2 8 1 7
1 2 6 1
7 4 7 5
6 1 3 8
10 10 4 3
</pre>
<h3>Example Output 2</h3>
<pre>5
</pre>