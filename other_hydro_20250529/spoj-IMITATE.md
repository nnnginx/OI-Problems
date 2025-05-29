<p>Iris is a student of ethology studying the animal behavior. She is interested by the imitation behavior of animals. Imitation is an advanced behavior whereby an individual observes and replicates another��s.</p>
<p>Iris is such a good researcher that she builds a mathematical model to describe the body figure of animals. She describes the body as a number of joints. And the figure or the status of animal body can be denoted as a set of ordered pairs of two different joints. To study the imitation of the animals, Iris defines the correlation of joints. She defines the correlation as the transitive closure of the ordered pairs of body status with its reflexive pairs eliminated. That is to say, the correlation is an anti-reflexive relation. In this case, we could say that one body status is imitating the other one when the correlations of both body statuses are the same.</p>
<p>For example, for the joint set {J1, J2, J3}. The first body status contains the ordered pair (J1, J2), (J2, J3). And the second body status contains the ordered pair (J1, J2), (J2, J3), (J1, J3). We could say that the first body status is imitating the other one because both of the correlation sets are (J1, J2), (J2, J3), (J1, J3) since the definition of the correlation is the transitive closure of body status.</p>
<p>For a given body status, that is, a given set of ordered pairs of joints, Iris want to get another body status, which is imitating the given one. At the same time, the desired body status must contain the minimum number of ordered pairs or the maximum number of ordered pairs. Your task is to calculate the minimum number and the maximum number.</p>
<h3>Input</h3>
<p>There are several test cases. The first line of the input contains a single integer denoting the number of test cases. There are about 100 test cases, but 90% of them are relatively small.</p>
<p>For each test case, the first line contains two integers <strong>N</strong> and <strong>M</strong> where <strong>N</strong> is the number of joints of both the given body status and the desired body status, <strong>M</strong> is the number of ordered pairs of the given body status. (1 &lt;= <strong>N</strong> &lt;= 1000, 0 &lt;= <strong>M</strong> &lt;= 10000)</p>
<p>Next <strong>M</strong> lines, each line denoting an ordered pair (<strong>X<sub>i</sub></strong>, <strong>Y<sub>i</sub></strong>). The <strong>X<sub>i</sub></strong> and <strong>Y<sub>i</sub></strong> are integers between 1 and N. Note that we consider the joints as the number between 1 and N.</p>
<h3>Output</h3>
<p>For each test case, output two integers denoting the minimum and maximum number of ordered pairs of the desired set. Two integers are separated by a single space.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
3 3
1 2
2 3
1 3
3 3
1 2
2 3
3 1
9 9
1 2
2 3
3 1
4 5
5 6
6 4
7 8
8 9
9 7

<strong>Output:</strong>
Case #1: 2 3
Case #2: 3 6
Case #3: 9 18
</pre>
<h3>Hint</h3>
<p>In mathematics, the transitive closure of a binary relation R on a set X is the transitive relation R+ on set X such that R+ contains R and R+ is minimal. If the binary relation itself is transitive, then the transitive closure will be that same binary relation; otherwise, the transitive closure will be a different relation.</p>
<p>A relation R on a set X is transitive if, for all x, y, z in X, whenever x R y and y R z then x R z. Examples of transitive relations include the equality relation on any set, the "less than or equal" relation on any linearly ordered set, and the relation "x was born before y" on the set of all people. Symbolically, this can be denoted as: if x &lt; y and y &lt; z then x &lt; z.</p>
<p>(From Wikipedia::transitive closure)</p>