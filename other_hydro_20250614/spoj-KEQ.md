<p>Every once in a while, Mishka Jabereen sends an interesting mathematical puzzle to his friends. This week's puzzle will be about so-called "repetitive" numbers иC the ones whose decimal expansion has just one kind of digit in it. (Examples of such numbers include 7, 11, and 5555.) The puzzle is about finding the largest repetitive number subject to two additional restrictions:</p>
<pre>(A) It must be divisible by at least one number from a given set. 
(B) It can not have more than a given number of digits.
</pre>
<p>A concrete example of such a problem statement would be: Find the largest repetitive number with at most 47 digits, which is divisible by 42 or 47! Mishka is currently playing around with a few such problem statements and he'd like to know all the answers, so that he can choose the nicest one.</p>
<h3>Problem specification</h3>
<p>A puzzle is described by a number K, the maximal number of digits allowed in the repetitive number, and a set of numbers d<sub>1</sub>, d<sub>2</sub>, бн, d<sub>R</sub>. Your task is to find the greatest repetitive number X that has at most K digits when written in decimal notation, and it is divisible by at least one of the d<sub>i</sub>.</p>
<h3>Input specification</h3>
<p>The first line of the input file contains an integer T specifying the number of test cases. Each test case is preceded by a blank line.</p>
<p>Each test case starts with a line containing the numbers K(1&lt;= K &lt;=10<sup>9</sup>) and R(1&lt;= R &lt;=7). The next R lines contain the numbers d<sub>i</sub>(1&lt;= d<sub>i</sub> &lt;=10<sup>14</sup>).</p>
<h3>Output specification</h3>
<p>We can describe a repetitive number by specifying its number of digits N and the digit D it contains.</p>
<p>For each test case, the output shall contain one line containing two integers N and D that describe the largest repetitive number that satisfies the conditions from the problem statement.</p>
<h3>Example</h3>
<pre><strong>input:</strong>
3

47 2
42
47

99 4
123
234
345
456

3 1
4700

<strong>output:</strong>
46 9
96 6
1 0
</pre>
<p>Note that in the third test case "3 0" would not be a correct answer, as "000" is not a valid integer.</p>
<p>This problem can be solved in a very short time but a naive solution may not terminate within 5 hours. Thanks to <a href="http://www.spoj.com/users/gerrob">Robert Gerbicz</a>'s help.</p>