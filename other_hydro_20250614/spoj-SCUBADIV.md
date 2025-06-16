<p align="justify">A scuba diver uses a special equipment for diving. He has a cylinder with two containers: one with oxygen and the other with nitrogen. Depending on the time he wants to stay under water and the depth of diving the scuba diver needs various amount of oxygen and nitrogen. The scuba diver has at his disposal a certain number of cylinders. Each cylinder can be described by its weight and the volume of gas it contains. In order to complete his task the scuba diver needs specific amount of oxygen and nitrogen. What is the minimal total weight of cylinders he has to take to complete the task? </p>

<h3>Example</h3>
<p align="justify">The scuba diver has at his disposal 5 cylinders described below. Each description consists of: volume of oxygen, volume of nitrogen (both values are given in litres) and weight of the cylinder (given in decagrams): </p>
<pre>3 36 120
10 25 129
5 50 250
1 45 130
4 20 119
</pre>
<p align="justify">If the scuba diver needs 5 litres of oxygen and 60 litres of nitrogen then he has to take two cylinders of total weight 249 (for example the first and the second ones or the fourth and the fifth ones).</p>

<h3>Task</h3>
<p align="justify">Write a program that for each test case:</p>
<div align="justify">
<ul align="justify">
        <li align="justify">reads scuba diver's demand for oxygen and nitrogen, the number of accessible cylinders and their descriptions; </li>
        <li align="justify">computes the minimal total weight of cylinders the scuba diver needs to complete his task; </li>
        <li align="justify">outputs the result. </li>
</ul>
</div>
<p align="justify"><b>Note:</b> the given set of cylinders always allows to complete the given task.</p>

<h3>Input</h3>
<p align="justify">The number of test cases <i>c</i> is in the first line of input, then <i>c</i> test cases follow separated by an empty line.</p>
<p align="justify">In the first line of a test case there are two integers <i>t</i>, <i>a</i> separated by a single space, 1 &lt;= <i>t</i> &lt;= 21 and 1 &lt;= <i>a</i> &lt;= 79. They denote volumes of oxygen and nitrogen respectively, needed to complete the task. The second line contains one integer <i>n</i>, 1 &lt;= <i>n</i> &lt;= 1000, which is the number of accessible cylinders. The following <i>n</i> lines contain descriptions of cylinders; <i>i</i>-th line contains three integers <i>t</i><i><sub>i</sub></i>, <i>a</i><i><sub>i</sub></i>, <i>w</i><i><sub>i</sub></i> separated by single spaces, (1 &lt;= <i>t</i><i><sub>i</sub></i> &lt;= 21, 1 &lt;= <i>a</i><i><sub>i</sub></i> &lt;= 79, 1 &lt;= <i>w</i><i><sub>i</sub></i> &lt;= 800). These are respectively: volume of oxygen and nitrogen in the <i>i</i>-th cylinder and the weight of this cylinder. </p>

<h3>Output</h3>
<p align="justify">For each test case your program should output one line with the minimal total weight of cylinders the scuba diver should take to complete the task. </p>

<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
5 60
5
3 36 120
10 25 129
5 50 250
1 45 130
4 20 119

<b><tt>Sample output:</tt></b>
249
</pre>