<p>Josu¨¦, one of the undergraduate students in PUCMM, is developing a Social Network, but he is having difficulties in identifying the person that has more possible friends. Two persons are possible friends if they are not friends and they have at least one common friend, for example if person A is friend only to person B, and person B is friend of C, then, A and C are possible friends. You are about to help him in this task. Given the network table, you have to write a program that finds the person that has more possible friends, if more than one person matches this criteria, then select the one that comes first ( the one that has the lower ID).</p>
<h3>Input</h3>
<p>The first line is <strong>T </strong>(1 ¡Ü <strong>T </strong>¡Ü 1,000), the number of test cases, then <strong>T</strong> test cases follow.</p>
<p>Each test case consists in a 'Y' or 'N' square matrix(<strong>M</strong>x<strong>M</strong>) representing the friendship of the network, where <strong>M</strong> is the number of persons.</p>
<pre><strong>Constraints</strong></pre>
<p><strong>M </strong>(1 ¡Ü <strong>M</strong> ¡Ü 50)</p>
<p>The square matrix has <strong>M</strong> lines, each line has <strong>M</strong> characters.</p>
<p>The first line of the matrix corresponds to person 0, the next line to person 1, and so on.</p>
<p>On each line the leftmost character corresponds to person 0, the next character to person 1, and so on.</p>
<p>So if character j of the line i is 'Y', it means that person 'i' is a friend of 'j'.</p>
<p>For each person i, character i of line i will be 'N'.</p>
<p>For each i,j character j of line i will be the same as character i of line j.</p>
<h3>Output</h3>
<p>For each test case, you have to output one line containing the ID of the person(0-based) that has more possible friends and the number of possible friends this person has, separated by a blank space.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>3<br>NYN<br>YNY<br>NYN<br>NYYY<br>YNNY<br>YNNN<br>YYNN<br>NNYNNNN<br>NNYNNNN<br>YYNYNNN<br>NNYNYNN<br>NNNYNYY<br>NNNNYNN<br>NNNNYNN<br><strong>Output:</strong><br>0 1<br>2 2<br>3 4</pre>