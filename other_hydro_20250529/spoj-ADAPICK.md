<p>Ada the Ladybug works as farmer. Its season of cucumbers and she wants to harvest them. There lies many cucumbers all around her house. She wants to choose a direction and follow it until all cucumbers in that direction are collected.</p>
<p>Lets consider Ada's house as centerpiece of whole universe, lying on <strong>[0,0]</strong>. The cucumbers are defined as lines on plane. No cucumber goes through Ada's house (and no cucumber touches it).</p>
<p>How many cucumbers can Ada pick in one go if she chooses the best direction possible?</p>
<h3>Input</h3>
<p>The first line contains an integer <strong>T</strong>, the number of test-cases.</p>
<p>Each test-case begins with an integer <strong>1 ¡Ü N ¡Ü 10<sup>5</sup> </strong></p>
<p>Afterward <strong>N</strong> lines follow, with four integers <strong>-10<sup>6</sup> ¡Ü     x<sub>1</sub>,y<sub>1</sub>,x<sub>2</sub>,y<sub>2</sub> ¡Ü     10<sup>6</sup></strong>, the beginning and end of each cucumber. Each cucumber         has positive length.</p>
<p>Sum of all <strong>N</strong> over all test-cases won't exceed <strong>10<sup>6</sup></strong></p>
<p>Even though cucumber will not go through house, they might touch, intersect or overlap other cucumbers!</p>
<h3>Output</h3>
<p>For each test-case print one integer - the maximal number of cucumbers which could be picked if Ada chooses a direction and picks every cucumber lying in it.</p>
<h3>Example Input</h3>
<pre>5
4
2 1 -1 4
-2 1 1 3
-3 2 0 5
-2 -2 5 1
3
-2 2 -2 -2
2 2 2 -2
-3 -3 -6 -3
3
-2 1 -3 4
3 1 5 5
-2 -2 2 -2
6
-1 5 -6 5
-3 -3 5 -3
-2 -5 5 -5
-1 -6 5 -6
5 1 5 5
6 6 6 -11
3
1 3 4 3
4 2 4 -1
5 1 6 6
</pre>
<h3>Example Output</h3>
<pre>3
2
1
4
2
</pre>
<h3>Possibly harvested cucumbers</h3>
<pre>1 2 3
1 3
1
2 3 4 6
2 3
</pre>