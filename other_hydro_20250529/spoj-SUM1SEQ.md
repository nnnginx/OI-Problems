<p align="justify">We say that a sequence of integers is a one-sequence if the difference between any two consecutive numbers in this sequence is 1 or -1 and its first element is 0. More precisely: [<i>a</i><sub>1</sub>, <i>a</i><sub>2</sub>, ..., <i>a<sub>n</sub></i>] is a one-sequence if

</p><div align="justify"><ul>
        <li align="justify">for any <i>k</i>, such that 1 &lt;= <i>k</i> &lt; <i>n</i> : |<i>a<sub>k</sub></i> - <i>a<sub>k</sub></i><sub>+1</sub>| = 1 and </li>
        <li align="justify"><i>a</i><sub>1</sub> = 0 </li>
</ul>
</div>

<h3>Task</h3>
<p align="justify">Write a program that for each test case:</p>
<div align="justify">
<ul align="justify">
        <li align="justify">reads two integers describing the length of the sequence and the sum of its elements; </li>
        <li align="justify">finds a one-sequence of the given length whose elements sum up to the given value or states that such a sequence does not exist; </li>
        <li align="justify">writes the result to the standard output.</li>
</ul></div>

<h3>Input</h3>
<p align="justify">The number of test cases <i>t</i> is in the first line of input, then <i>t</i> test cases follow separated by an empty line.</p>
<p align="justify">In the first line of a test case there is a number <i>n</i>, such that 1 &lt;= <i>n</i> &lt;= 10 000, which is the number of elements in the sequence. In the second line there is a number <i>S</i>, which is the sum of the elements of the sequence, such that |<i>S</i>| &lt;= 50 000 000. </p>

<h3>Output</h3>
<p align="justify">For each test case there should be written <i>n</i> integers (each integer in a separate line) that are the elements of the sequence (<i>k</i>-th element in the <i>k</i>-th line) whose sum is <i>S</i> or the word "No" if such a sequence does not exist. If there is more than one solution your program should output any one.</p>
<p align="justify">Consequent test cases should by separated by an empty line.</p>

<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
8
4

<b><tt>Sample output:</tt></b>
0
1
2
1
0
-1
0
1
</pre>