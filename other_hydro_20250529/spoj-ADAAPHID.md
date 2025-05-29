<p>Ada the Ladybug breeds aphids. Whenever a new aphid is born, she assigns him an ID. She did that for long time but as she can't remember tha ID's she sometime made duplicates. She wanted to avoid such situation so she extended the ID to pair. She has also chosen a random number, which she assigned to aphid and then she made second integer of ID as sum of values of all aphids with ID lesser or equal to current ID (including current ID).</p>
<p>She wants to know the ID of each aphid. Please, read the input section carefully.</p>
<h3>Input</h3>
<p>The first line contains <strong>1 ¡Ü  Q ¡Ü 3*10<sup>5</sup> </strong>, number of aphids added.</p>
<p>Let <strong>L</strong> be the second integer of last aphid's ID (beggining with 0).</p>
<p>The next <strong>Q</strong> lines contains two numbers <strong>A, V</strong>, <strong>0 ¡Ü A, V     &lt; 2<sup>60</sup></strong>, where <strong>A ¨’ L</strong> is the first integer of aphid's ID and <strong>V ¨’ L</strong> is the random number (<strong>¨’</strong> stands for XOR).</p>
<p><strong>1 ¡Ü A ¨’ L &lt; 2<sup>60</sup></strong></p>
<p><strong>1 ¡Ü V ¨’ L &lt; 1000</strong></p>
<h3>Output</h3>
<p>For each query print both number's of aphid's ID.</p>
<h3>Example Input</h3>
<pre>7
1 1
3 3
4 0
3 2
5 6
13 13
19 19
</pre>
<h3>Example Output</h3>
<pre>1 1
2 3
7 6
5 7
2 4
9 20
7 18
</pre>
<h3>Input after XOR</h3>
<pre>7
1 1
2 2
7 3
5 4
2 1
9 9
7 7
</pre>