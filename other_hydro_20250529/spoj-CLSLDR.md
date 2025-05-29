<p>This is new year in Planet X and there is something special! A classroom in this planet is looking for a new class leader using an unique game!<br><br>These are the ways how the game is played.<br>1. There are <strong>n</strong> students in the class. Each student is labeled from 1 (first student) to <strong>n</strong> (last student).<br>2. A paper is given to <strong>m</strong>-th student.<br>3. The next <strong>o</strong>-th student who gets the paper quits the game.<br>4. The paper is passed until there is one last student who hasn't quitted the game.<br>5. The student becomes the class leader.<br><br>Now, your task is to find the number of such student.</p>
<h3>Input</h3>
<p>The first line contains a number <strong>T</strong> (0 &lt;= T &lt;= 10<sup>6</sup>).<br>Each of the next <strong>T</strong> lines contains 3 integers which are <strong>n</strong> (0 &lt; n &lt;= 10<sup>3</sup>), <strong>m</strong>, <strong>o</strong> (0 &lt; m, o &lt;= n) and are separated by a single space.</p>
<h3>Output</h3>
<p>For each test cases, print the required answer.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>4 1 2<br>5 2 3

<strong>Output:</strong>
2<br>1<br><br></pre>
<p><span style="font-size: small;"><strong>Explanation for test case 1</strong></span></p>
<p>1 2 3 4 -&gt; The paper is being held by student 1. Pass the paper by 2 students. Now, the paper is being held by student 3.<br>1 2 4&nbsp;&nbsp;&nbsp; -&gt; Student 3 quits. Pass the paper by 2 students. Now, the paper is being held by student 1.<br>2 4&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; -&gt; Student 1 quits. Pass the paper by 2 students. Now, the paper is being held by student 4.<br>2&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp; -&gt; Student 4 quits. Student 2 becomes the class leader.</p>
<p>&nbsp;</p>