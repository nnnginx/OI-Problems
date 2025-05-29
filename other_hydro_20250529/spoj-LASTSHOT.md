<p>Tony Stark is on the mission to save the world from Loki's army so he spread N bombs in the enemy region. He spread the bombs in such a way that a bomb can be in range of another bomb i.e say bomb B1 is in range of bomb B2 , when bomb B2 explodes it will trigger bomb B1 and it also get explode but vice-versa might not be true because the bombs are of different of range. As he is running out of energy so he left with one shot&nbsp;To trigger the bomb .Now he ask Jarvis to find most appropriate bomb which he can trigger to make maximum impact.</p>
<p>Impact is basically number of bombs get explode.</p>
<p>Can you help Jarvis to do so?</p>
<h3>Input</h3>
<p>First line contains two integer N and M denoting number of bombs and number of relation between the bombs.</p>
<p>1 ¡Ü n ¡Ü 10000</p>
<p>1 ¡Ü m ¡Ü 10000</p>
<p>Next M lines contain two integer A and B denoting bomb B is in range of bomb A.</p>
<p>1 ¡Ü A ¡Ü N</p>
<p>1 ¡Ü B ¡Ü N</p>
<h3>Output</h3>
<p>A single line containing MAXIMUM IMPACT.</p>
<h3>Example 1</h3>
<pre><strong>Input:</strong>
4 3
1 2
2 4
1 3
<strong>Output:</strong>
4</pre>
<h3>Example 2</h3>
<pre><strong>Input:</strong>
4 3
1 2
2 1
2 3
<strong>Output:</strong>
3</pre>