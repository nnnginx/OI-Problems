<p align="justify">A diskette was enclosed to a road map. The diskette contains the table of the shortest ways (distances) between each pair of towns on the map. All the roads are two-way. The location of towns on the map has the following interesting property: <i>if the length of the shortest way from town A to town B equals the sum of the lengths of the shortest ways from A to C and C to B then town C lies on (certain) shortest way from A to B</i>. We say that towns A and B are neighbouring towns if there is no town C such that the length of the shortest way from A to B equals the sum of the lengths of the shortest ways from A to C and C to B. Find all the pairs of neighbouring towns. </p>

<h3>Example</h3>
<p align="justify">For the table of distances: </p>
<table>
        <tbody><tr>    <th></th><th>A</th><th>B</th><th>C</th>         </tr>
        <tr>    <th>A</th><td>0</td><td>1</td><td>2</td>        </tr>
        <tr>    <th>B</th><td>1</td><td>0</td><td>3</td>        </tr>
        <tr>    <th>C</th><td>2</td><td>3</td><td>0</td>        </tr>
</tbody></table>
<p align="justify">the neighbouring towns are A, B and A, C. </p>

<h3>Task</h3>
<p align="justify">Write a program that for each test case:</p>
<div align="justify">
<ul align="justify">
        <li align="justify">reads the table of distances from standard input; </li>
        <li align="justify">finds all the pairs of neighbouring towns; </li>
        <li align="justify">writes the result to standard output. </li>
</ul>
</div>

<h3>Input</h3>
<p align="justify">The number of test cases <i>t</i> is in the first line of input, then <i>t</i> test cases follow separated by an empty line.</p>
<p align="justify">In the first line of each test case there is an integer <i>n</i>, 1 &lt;= <i>n</i> &lt;= 200, which equals the number of towns on the map. Towns are numbered from 1 to <i>n</i>.</p>
 <p align="justify">The table of distances is written in the following <i>n</i> lines. In the (<i>i</i>+1)-th line, 1 &lt;= <i>i</i> &lt;= <i>n</i>, there are <i>n</i> non-negative integers not greater than 200, separated by single spaces. The <i>j</i>-th integer is the distance between towns <i>i</i> and <i>j</i>. </p>

<h3>Output</h3>
<p align="justify">For each test case your program should write all the pairs of the neighbouring towns (i.e. their numbers). There should be one pair in each line. Each pair can appear only once. The numbers in each pair should be given in increasing order. Pairs should be ordered so that if the pair (<i>a</i>, <i>b</i>) precedes the pair (<i>c</i>, <i>d</i>) then <i>a</i> &lt; <i>c</i> or (<i>a</i> = <i>c</i> and <i>b</i> &lt; <i>d</i>).</p>
<p align="justify">Consequent test cases should by separated by an empty line.</p>

<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
3
0 1 2
1 0 3
2 3 0

<b><tt>Sample output:</tt></b>
1 2
1 3
</pre>