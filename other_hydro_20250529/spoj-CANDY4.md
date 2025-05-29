<p>Lazy Child is a lazy child who likes candy very much. Despite being very young, he has two large candy boxes, each initially containing <strong>n</strong> candies. Everyday he picks one box and open it, if there still are candies, he would eat one. If not, he would be quite sad and open the other box. He will pick the first box with probability <em>p</em> and the second box with probability 1-<em>p</em>. He might cry if the other box contains few candies.</p>
<p>He opens a box and finds it's not empty, then takes out 1 candy from it and eats it for several days, while he can't remember how many days are there exactly. One day, he opens a box, only to find no candy left. Before opening the other box, he wants to know the expected number of candies left in the other box. Can you help him?</p>
<h3>Input</h3>
<p>There are several test cases (about 100), please process till EOF.</p>
<p>Each of the following lines contains an integer <strong>n</strong> (1&lt;= <strong>n</strong> &lt;= 20000) and a real number <strong>p</strong> (0 &lt;= <strong>p</strong> &lt;= 1, with 6 digits after the decimal).</p>
<h3>Output</h3>
<p>Please print one line per case containing the desired answer. Any answer with an absolute error less than or equal to 10<sup>-2</sup> would be accepted. Please see the sample output for detailed format.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
10 0.400000
100 0.500000
124 0.432650
325 0.325100
532 0.487520
2276 0.720000

<strong>Output:</strong>
Case 1: 3.528175
Case 2: 10.326044
Case 3: 28.861945
Case 4: 167.965476
Case 5: 32.601816
Case 6: 1390.500000
</pre>