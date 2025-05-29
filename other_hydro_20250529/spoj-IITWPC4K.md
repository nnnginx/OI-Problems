<p>Until now you would have known that Maggu is a big geek. His class has n students. All the students are geeks like him. You are given m informations of form a, b which denotes that a th guy is less geeky than b th guy (geekiness(a) &lt; geekiness (b)). Note that geekiness of each person is unique and can be from 1 to n. Now Maggu wonders what are the possible values of his geekiness. If such a distribution of geekiness value is not possible, then output -1.&nbsp;</p>
<h3>Input</h3>
<p>First line contains T: number of test cases (1 &lt;= T &lt;= 100).</p>
<p>For each test case, first line contains n, m, idx where n is number of boys in the class, m is number of informations, idx is the index corresponding to Maggu. 1 &lt;= n &lt;= 10^6, 1 &lt;= m &lt;= min (10^5, n * (n - 1) / 2), 1&lt;= idx &lt;= n.</p>
<p>Then next m line contains two space separated integers representing a, b. (1 &lt;= a, b &lt;= n).</p>
<p>No pair of information is repeated twice in the input.</p>
<h3>Output</h3>
<p>For each test case, You have to output one or two lines depending on the situation. In the former case, If the &nbsp;disribution of geekiness can not exist, output -1.</p>
<p>In the second case (ie two lines), In the first line, output a single integer number of possible geekiness values of Maggu.<br>Then in the next line output in the increasing order all the possible geekiness values of Maggu in ascending order. All the values should be space seperated.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>3 2 1<br>1 2<br>2 3<br>4 2 1<br>1 2<br>3 4

<strong>Output:</strong>
1<br>1<br>3
1 2 3</pre>