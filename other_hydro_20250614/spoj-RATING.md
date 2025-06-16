<p>Some of the more elite (and not-so-elite) coders around take part in a certain unnamed programming contest. In said contest, there are multiple types of competitions. Here, we consider the Open and High School competition types. For each type, each competitor receives a <em>rating</em>, an integer between 1 and 100000, inclusive. A coder's rating is based upon his or her level of performance in matches and is calculated using a complicated formula which, thankfully, you will not be asked to implement.<br> <br> Although the Open and High School ratings for a coder who has participated in both competition types lately are usually close, this is not always the case. In particular, High School matches are more about speed, since many coders are able to solve all the problems, whereas Open matches require more thinking and there is a steeper curve in terms of problem difficulty.<br> <br> <strong>Problem Statement</strong><br> You are given <em>N</em> coders (1 ¡Ü <em>N</em> ¡Ü 300000), conveniently numbered from 1 to <em>N</em>. Each of these coders participates in both High School and Open matches. For each coder, you are also given an Open rating <em>A<sub>i</sub></em> and a High School rating <em>H<sub>i</sub></em>. Coder <em>i</em> is said to be <em>better</em> than coder <em>j</em> if and only if both of coder <em>i</em>'s ratings are greater than or equal to coder <em>j</em>'s corresponding ratings, with at least one being greater. For each coder <em>i</em>, determine how many coders coder <em>i</em> is better than.<br> <br> <strong>Input Format</strong><br> On the first line of input is a single integer <em>N</em>, as described above.<br> <em>N</em> lines then follow. Line <em>i</em>+1 contains two space-separated integers, <em>A<sub>i</sub></em> and <em>H<sub>i</sub></em>.<br> <br> <strong>Output Format</strong><br> Line <em>i</em> should contain the number of coders that coder <em>i</em> is better than.<br> <br> <strong>Sample Input</strong></p>
<pre>8
1798 1832
862 700
1075 1089
1568 1557
2575 1984
1033 950
1656 1649
1014 1473
</pre>
<p>&nbsp;</p>
<p><strong>Sample Output</strong></p>
<pre>6
0
2
4
7
1
5
1</pre>
<p>&nbsp;</p>