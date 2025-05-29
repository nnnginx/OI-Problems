<p>Recently, Jimmy is learning about linear algebra from Blue Mary while having the course of Boolean algebra in class offered by Prof. Z. Since Jimmy has been thoroughly bored by the boring homework assigned by two teachers, evil Jimmy plans to set a hard question to baffle them as revenge for their heavy tasks. As a result, Jimmy comes up with an idea that merging the knowledge from both the two classes and constructs a complicate problem: the XOR equation system.</p>
<p>Let's consider the following equations:</p>
<p><img src="../../../content/john_jones:xoreq1.jpg" alt=""></p>
<p>which satisfies the following conditions:</p>
<p><img src="../../../content/john_jones:xoreq2.jpg" alt=""></p>
<p>In the system of equations, operation <strong>.</strong> denotes the multiplication operation while <strong>^</strong> is for bitwise XOR. Moreover, the bitwise XOR takes two bit patterns of equal length and performs the logical XOR operation on each pair of corresponding bits. The result in each position is 1 if the two bits are different, and 0 if they are the same.</p>
<p>Rather than expecting a solution of a specified equation system, Jimmy would like to ask the teachers to calculate that how many distinct solutions can satisfy a given equation system. What a confusing puzzle! Help Jimmy's teachers please!</p>
<h3>Input</h3>
<p>There are several test cases. The first line of input is a single positive integer (&lt;= 15) indicating the number of test cases, the test cases follow.</p>
<p>For each test case, the first line contains two integers <strong>N</strong> and <strong>M</strong> giving the two dimensions of the equation system respectively where <strong>N</strong> is the number of rows and <strong>M</strong> for columns. Then <strong>N</strong> lines are following, each line contains <strong>M</strong> integers. Item at line <em>i</em> and column <em>j</em> represents a<sub>ij</sub>. The next <strong>M</strong> lines are descriptions of S<sub>i</sub> that the leading integer <strong>K</strong> denotes the number of elements in S<sub>i</sub> and the following <strong>K</strong> integers represent elements.</p>
<h3>Output</h3>
<p>For each test case, output one line containing a single integer which represents the answer of this case.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
1 2
1 1
3 0 1 2
2 3 1

<strong>Output:</strong>
1
</pre>