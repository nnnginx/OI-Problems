<p>One of your friends was in relationship with multiple people at once and it didn¡¯t end very well. Thus he/she chose the path of righteousness and decided to stay in only one relationship or stay single. But not only that, he/she became a motivational speaker and formed an organization to help people to walk through this path.</p>
<p>N people joined his/her organization. He/She takes one person and he/she either pairs that person up with another person in a relationship or keeps that person single. Let¡¯s assume that every person can be paired up with every other person. In how many ways he/she can do that?</p>
<h3>Input</h3>
<p>First line of input will be T (1&lt;= T &lt;= 100000), denoting the number of test cases.</p>
<p>Next T lines will contain one integer N (1&lt;= N &lt;= 100000) per line.</p>
<h3>Output</h3>
<p>For each test case print correct answer describe in the description. As, output can be large. Print it modulo 1000000007.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
3
100000

<strong>Output:</strong>
4
823421181
</pre>
<h3>Explanation</h3>
<p>For case one, let¡¯s assume they are numbered 1 2 and 3.</p>
<p>Formation can be:</p>
<p>{1} {2} {3} // every person is single</p>
<p>{1} {2, 3} // one is single and two other is in a relationship</p>
<p>{1, 2} {3} // one is single and two other is in a relationship</p>
<p>{1, 3} {2} // one is single and two other is in a relationship</p>
<p>Thus answer is 4.</p>