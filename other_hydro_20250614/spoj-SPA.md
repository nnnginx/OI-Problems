<p><em>Original problem statements can be found here: <a href="https://contest.pizza/static/tasks/2018/eliminations/statki.pdf">in Polish</a> and <a href="https://contest.pizza/static/tasks/2018/eliminations/statki_en.pdf">in English</a></em>.</p>

<p>Aliens attack! Run for your lives!</p>

<p>... or not, it's only a video game. And even then, although alien spaceships are flying straight for the Earth, it's not terribly important to destroy them all. Gregory the Gamer only wants that sweet high score.</p>

<p>To be more precise, there are <strong>n</strong> enemy spaceships, flying in a row. Every spaceship is of one of three colours. Our own spaceship is flying opposite of those, from left to right, and can destroy any of them. Destroying a spaceship of colour i is worth p<sub>i</sub> points. If you destroy more than one spaceship of the same color in a row, you get more points - second spaceship in sequence is worth 
2p<sub>i</sub> points, for the third one you get 3p<sub>i</sub> and so on. The maximum number of points you can get for one spaceship is limited by <strong>M</strong> - if the previous rule dictates more than that, you get exactly <strong>M</strong> points instead.</p>

<p>What is the highest score Gregory can get?</p>
<h3>Input</h3>
<p>The first line contains a single integer <strong>t</strong>, denoting number of testcases. Then, testcases follow.</p>

<p>The first line of a testcase contains two integers <strong>n</strong>, <strong>M</strong> - number of spaceships and points limit for one spaceship (  1 &lt;= <strong>n</strong> &lt;= 10<sup>5</sup>, 1 &lt;= <strong>M</strong> &lt;= 100  ).</p>

<p>In the next line there are three integers  1 &lt;= <strong>p<sub>A</sub></strong>, <strong>p<sub>B</sub></strong>, <strong>p<sub>C</sub></strong> &lt;= <strong>M</strong>  - point values for destroying spaceships of different colours.</p>

<p>In the last line there is a string of length <strong>n</strong> - description of subsequent spaceships. Every character is one of the following: A, B, C. Different characters correspond to different colours.</p>

<h3>Output</h3>
<p>For every testcase you should output one integer - highest score you can get.</p>

<h3>Example</h3>
<p>Input:</p>
<pre>2
7 5
1 1 5
AAACAAA
6 10
1 1 10
ABABAB</pre>
<p>Output:</p>
<pre>20
7</pre>

<h3>Explanation</h3>
<p>In the first testcase we destroy all six spaceships of colour A, and we get  1+2+3+4+5+5 = 20  points. If we destroyed all of them instead, we'd get (1+2+3)+5+(1+2+3) = 17 points.</p>

<p>In the second testcase we can first destroy all spaceships of colour A, and then the last spaceship of colour B, which will give us (1+2+3)+1 = 7.</p>