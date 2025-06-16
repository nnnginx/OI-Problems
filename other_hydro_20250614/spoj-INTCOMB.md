<p>You will be given n positive integers a_1, a_2, ..., a_n. We say that a  nonnegative integer combination of these numbers is of the form a_1*b_1 +  a_2*b_2 + ... + a_n*b_n where each of b_1, b_2, ..., b_n is a  nonnegative integer. You are to determine how many positive integers  cannot be expressed as a nonnegative integer combination of a_1, a_2,  ..., a_n.</p>
<h3>Input</h3>
<p>The first line contains a single integer denoting the number of test  cases (about 30). Each test case consists of a single line. The first  integer on the line is n, between 1 and 30, which indicates the number  of integers a_1, a_2, ..., a_n. Then n integers follow each between 1  and 100,000. The i'th such integer is a_i. All integers on this line are  separated by a space.</p>
<h3>Output</h3>
<p>For each test case you are to output a single line. If there are only a  finite number of positive integers that cannot be expressed as a  nonnegative integer combination of a_1, a_2, ..., a_n, then you are to  output this number. Otherwise, simply output the text "Infinite"  (without quotes).</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>3 <br>2 2 4 <br>2 4 5 <br>3 11 12 13<br><strong>Output:</strong>
Infinite <br>6 <br>30<br><strong>Explanation<br></strong>Sample Test 2 :<br>You cannot express 1,2,3,6,7 and 11 using only the integers 4 and 5.<br><strong><br></strong></pre>
<h3>Constraints</h3>
<p>1 &lt;= n &lt;= 30 <br> 1 &lt;= a_i &lt;= 100000</p>