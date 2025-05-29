<p>Little Gopu likes to play very much. As you know he only plays with numbers. So he is given n numbers. Now he tries to group the numbers into collections where each collection contains exactly two numbers. He can form the collection of two numbers a and b (a &lt;= b), if and only if b is either 2 * a or 2 * a + 1.</p>
<p>Note that you can not use a single number in forming of more than one collections. Eg. 1, 2, 4 He can divide the numbers into a single collection only either [1, 2] or [2, 4] because each collection requires exactly two numbers, and each number has to be used only once in a group.</p>
<p>Given n numbers, Find out how many maximum number of collections he can form ?</p>
<h3>Input</h3>
<p>T: number of test cases.</p>
<p>For each test case, First line will contain n :&nbsp; (1 &lt;= n &lt;= 10^5)</p>
<p>Then next line will contain n numbers single space seperated. Range of each number will be between 1 and 10^18.</p>
<p>Sum of n over all the tests will be atmost 10^6. So number of test cases are decided on this criteria.</p>
<h3>Output</h3>
<p>For each test case, output maximum number of collections that can be formed.</p>
<h3>Example</h3>
<pre><strong>Input:<br></strong>4<br>2<br>1 2<br>3 <br>1 2 4<br>4<br>1 2 4 8<br>2<br>4 4&nbsp;</pre>
<pre><strong>Output:<br></strong>1<br>1<br>2<br>0&nbsp;</pre>