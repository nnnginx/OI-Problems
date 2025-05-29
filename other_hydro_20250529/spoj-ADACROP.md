<p>As you might already know, Ada the Ladybug is a farmer. She has a very long furrow with many kinds of vegetables (represented by integer numbers). Whenever she wants to harvest a single vegetable, she always replace it with anoher vegetable (possibly same kind).</p>
<p>After each replacement, she wants to know the number of vegetables of the same kind (at the new vegetable) which are before it (have lower possition in furrow).</p>
<p></p>
<h3>Input</h3>
<p>The first line of input containts  <strong>1 ¡Ü N, Q ¡Ü 2*10<sup>5</sup> </strong>, the length of furrow and number of harvests.</p>
<p>The next line contains <strong> N </strong> numbers  <strong>0 ¡Ü A<sub>i</sub> ¡Ü     10<sup>9</sup></strong> the kind of vegetable which is currently on <strong>i<sup>th</sup></strong> spot in furrow (indexed from 0).</p>
<p>The next <strong>Q</strong> lines contains two numbers <strong>0 ¡Ü i &lt; N</strong> (the index of harvested plant) and <strong>0 ¡Ü a ¡Ü 10<sup>9</sup></strong> (the kind of newly planted vegetable)</p>
<h3>Output</h3>
<p>For each harvest, print the number of vegetables of the same kind before the newly planted vegetable.</p>
<h3>Example Input</h3>
<pre>5 5
1 2 1 2 1
2 2
4 2
2 3
3 3
4 3

</pre>
<h3>Example Output</h3>
<pre>1
3
0
1
2
</pre>
<h3>Example Input 2</h3>
<pre>10 10
2 3 5 3 9 3 5 2 9 9
7 2
0 5
0 2
1 2
9 2
4 3
8 2
4 2
2 5
3 5
</pre>
<h3>Example Output 2</h3>
<pre>1
0
0
1
3
1
3
2
0
1
</pre>