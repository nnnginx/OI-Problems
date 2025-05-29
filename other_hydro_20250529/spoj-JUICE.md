<p>Jerry loses himself in the interesting game: Fruit Ninja. Fruit Ninja is a game of iPhone and iPad in which the players cut the fruits coming from the bottom of the screen and gain the bonus from cutting more than two fruits with a single slice. Once a fruit is cut, it breaks into small pieces and cannot be cut any more.</p>
<p>After months of training, he becomes pro of this game. Actually, he can cut all the fruits on the screen at any time. Jerry also has a bad habit that he has no willing to leave some fruits for the future cutting. In the other words, after Jerry cuts the fruits, all the fruits on the screen breaks and no one left. That is why all his friends call him <em>Juice Extractor</em>.</p>
<p>Now he only consider about the bonus, when he cuts more than two fruits, he can gain some bonus scores as same as the number of fruits he slice at that time. For example, if Jerry cuts 4 fruits with a single slice, he can get 4 scores from this slice.</p>
<p>After Jerry gets the fruit schedule, he knows the appearing time and the disappearing time for every single fruit. He can only cut a fruit into pieces between its appearing time and disappearing time inclusive. He wants to know the maximum possible bonus scores he can receive.</p>
<h3>Input</h3>
<p>There are several test cases; the first line of the input contains a single integer <strong>T</strong>, denoting the number of the test cases. (<strong>T</strong> &lt;= 200)</p>
<p>For each test case, the first line contains an integer <strong>N</strong>, denoting the total number of fruits. (1 &lt;= <strong>N</strong> &lt;= 1000)</p>
<p>The next <strong>N</strong> lines, each line describe a fruit. For each line, there are two integers <strong>X<sub>i</sub></strong> and <strong>Y<sub>i</sub></strong>, where <strong>X<sub>i</sub></strong> is the appearing time of the fruit and <strong>Y<sub>i</sub></strong> is the disappearing time of this fruit. (0 &lt;= <strong>X<sub>i</sub></strong> &lt;= <strong>Y<sub>i</sub></strong> &lt;= 1000000000)</p>
<h3>Output</h3>
<p>For each test case, output a single integer denoting the maximum scores that Jerry could possibly gain. See the sample for further details.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
10
1 10
2 11
3 12
4 13
13 14
14 15
13 19
20 22
21 23
22 24

<strong>Output:</strong>
Case #1: 10
</pre>