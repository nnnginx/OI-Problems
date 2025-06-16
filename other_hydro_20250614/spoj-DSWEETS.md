<p>One day AAST students had their marks in ¡°Scientific Thinking¡± and most of students had bad marks.</p>
<p>So the lecturer want to give them something to make them happy so he checked his bag and found n sweets, so he decided to distribute them to his students by this way:</p>
<p>1-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Everyone gets an integer number of sweets and at least one sweet.</p>
<p>2-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; He wanted the ratio between mark of a student and number of sweets this student gets equal to the ratio between these of any other student. (for all students: mark of a student / number of sweets he gets = constant, where number of sweats he gets are more than zero and this constant could be any real number).</p>
<p>3-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; It must be distributed following last conditions such that no sweets remain.</p>
<p>Example: if two students x and y, x has 5 marks and y has 10 marks, so y must get double the number of sweets x will get which is the number of sweets x will get is at least one.</p>
<p>But Mohamed Ramzy is the most student joking in his lecture so that he decided to punish him and asked him to distribute the sweets, but Ramzy doesn¡¯t know if it is possible to distribute the sweets following the conditions the lecturer stated so he asked you to help him.&nbsp;</p>
<h3>Input</h3>
<p>First line contains an integer t, the number of test cases.</p>
<p>For each test case , it begins with two integers n and m, the number of sweets and the number of students respectively. The next line contains m integers, the marks of the students, such that the first mark belongs to the first student , the second mark belongs to the second students and so on¡­</p>
<p>Edit: There is no blank line in the input file</p>
<h3>Output</h3>
<p>For each test case print one line: ¡°YES¡± if it is possible to distribute it following the conditions, ¡°NO¡± otherwise.</p>
<h3>Constraints</h3>
<pre>0 &lt;= n &lt;= 1000000
0 &lt; m &lt;= 1000000
0 &lt;= mark of each student &lt;= 1000000
</pre>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
5 4
1 1 1 1
4 4
1 1 1 1
3 2
1 2

<strong>Output:</strong>
NO
YES
YES
</pre>
<h3>Explanation</h3>
<p>First test case there is no possible way to distribute the sweets following the conditions stated.</p>
<p>In the second and third test case it is possible <span style="white-space: pre;">to distribute the sweets</span> such that the constant will be one.</p>