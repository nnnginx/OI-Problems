<p>In Dystopia, chocolates are being distributed to children waiting in a queue. The distribution proceeds as follows. Each chocolate bar is rectangular in shape with integer edge lengths. If the chocolate bar is a square, it is given away completely to the first child in the queue. Otherwise the largest possible square piece of chocolate is broken off from the chocolate bar and given to the first child. After a child receives his share of chocolate, he leaves the queue. The remaining portion of the chocolate bar is dealt with in the same fashion and the whole or a portion of it is given to the next child in the queue.</p>
<p>For example, if we start with a 5x3 chocolate bar, the first child in the queue receives a 3x3 chocolate bar, leaving a 2x3 bar. The second child gets a 2x2 bar while the third and fourth children get 1x1 bars. Thus four children have been fed using the 5x3 bar.</p>
<p>The Dystopian government has got a carton of chocolate bars to be distributed to children in the country. To make sure that maximum inequality is achieved while distributing chocolates, the chocolate bars in the carton are all of different sizes. For every i such that M&lt;=i&lt;=N and every j such that P&lt;=j&lt;=Q (where M,N,P,Q are integers) there is exactly one chocolate bar of length i and breadth j in the carton. Here a bar of length i and breadth j is considered to be different from a bar of length j and breadth i.</p>
<p>Given the values of M,N,P,Q find the number of children that can be fed with the chocolate in the carton.</p>
<h3>Input</h3>
<p>The first line of the input contains the number of test cases, T (&lt;=1000)</p>
<p>Following this are T lines, each describing a test case with four integers M,N,P,Q separated by spaces (1&lt;=M&lt;=N&lt;=100000000, 1&lt;=P&lt;=Q&lt;=1000)</p>
<h3>Output</h3>
<p>Output T lines, each containing an integer : The number of children that can be fed using the chocolate in the carton</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
1 2 1 2
3 4 4 5

<strong>Output:</strong>
6
14
</pre>