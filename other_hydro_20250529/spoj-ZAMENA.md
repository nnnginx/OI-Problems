<p>Little Picsel, a long-term member of the Secret Committee, has decided to resign after years of loyal service. However, as he does not want his departure to go unnoticed, he has decided to encrypt his final suggestion for this year's Nationals, using a key only known to him. He left only a single array to the other Committee members, containing all of their IDs (<strong>the IDs are of a fixed length and need not be unique</strong>), and the statement of the problem that they must solve in order to obtain the key:</p>
<p>Picsel had initially traversed the array, starting from the first element towards the last, until he found an ID he liked and remembered it. Then he continued his traversal, and upon encountering a very similar ID to the one he remembered (two IDs are <em>very similar</em> if they differ <strong>at most in a single digit</strong>), he has two options:</p>
<ul>
<li><strong>remembering the encountered ID</strong> instead of the previously remembered one, and continuing his traversal;</li>
<li><strong>continuing his traversal</strong> <strong>without remembering the encountered ID</strong>.</li>
</ul>
<p>Picsel also keeps track of the total 'score' he has obtained throughout his traversal; initially, his score is set to zero, however whenever he chooses to remember a new ID, <strong>the score increases by the absolute difference of the old and new ID's digit on the position in which they differ</strong>. For example, if the previously remembered ID was 1234, and the newly remembered ID is 1274, the score increases by 4 in that case. The Committee now must determine the <strong>maximal score</strong> that Picsel could have achieved.</p>
<p>The Nationals have already begun, and the Committee had failed to decrypt Picsel's problem and are unable to offer the contestants a new one. As such, they asked for your help with the decryption; for additional motivation, they are offering you 100 points at the contest as a reward.</p>
<h3>Input</h3>
<p>The first line of the standard input contains a natural number N, representing the amount of members of the Secret Committee.</p>
<p>Each of the following N lines contains a single integer A<sub>i</sub>, representing the ID of the i-th committee member in the array.</p>
<h3>Output</h3>
<p>Write to the first and only line of the standard output a single integer M, representing the maximal score that Picsel could have achieved.</p>
<h3>Example</h3>
<pre><strong>Input:<br></strong>6<br>8823<br>2145<br>2185<br>3385<br>4145<br>4445</pre>
<pre><strong>Output:</strong>
5</pre>
<h3>Explanation</h3>
<p>Picsel first decides to remember the ID 2145. Afterwards he immediately has the option of remembering 2185 instead, however he refuses to do so, as if he were to choose to remember the ID 4145 instead, followed immediately by 4445, he would win a total score of 5:</p>
<p>2145 -&gt; 4145 -&gt; 4445 =&gt; score = |4 - 2| + |4 - 1| = 5</p>
<p>There is no strategy that will result in Picsel scoring more than five points.</p>
<h3>Constraints</h3>
<ul>
<li>1 &lt;= N &lt;= 10<sup>5</sup></li>
<li>0 &lt;= A<sub>i</sub>&nbsp;&lt; 10<sup>7</sup></li>
<li>All of the IDs A<sub>i</sub>&nbsp;will be of the same length</li>
</ul>