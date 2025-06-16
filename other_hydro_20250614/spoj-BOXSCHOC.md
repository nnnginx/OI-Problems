<p>Choco-moo has gone to the super market to buy chocolates for his friends. He entered a shop and found that they sell many boxes of chocolates. All the chocolate boxes are lined up on the display and there are exactly <strong>N (0 &lt; N &lt;= 100000) </strong>chocolate boxes. The i-th number box contains <strong>A</strong>i <strong>(0 &lt; Ai &lt;= 100000) </strong>amount of chocolates inside. Choco-moo loves chocolates and wants to buy all of the boxes, but he won��t. He will only buy boxes that contains amount of chocolates that can be divided by <strong>K</strong> <strong>(0 &lt; K &lt;= 100000) </strong>since he has K number of friends and wants to divide the chocolates equally without wasting any chocolates.</p>
<p>Now, you are given the value N and then N numbers indicating the amount of chocolates inside the N boxes. You have to answer some queries for Choco-moo. You will be given <strong>Q</strong> <strong>(0 &lt; Q &lt;= 100000)</strong> queries.</p>
<p>In each query, Choco-moo will provide you with three integers, <strong>A</strong>, <strong>B</strong>&nbsp; <strong>(0 &lt; A&lt;=B &lt;= N) </strong>and K. Here A and B are index number and K is the number of friends Choco-moo has. Now you have to find how many chocolate boxes Choco-moo can buy between Ath box to Bth box (inclusive)?</p>
<h3>Input</h3>
<p>The first line contains an integer <strong>T</strong> (<strong>T</strong>&lt;=2), which is the number of test cases.</p>
<p>Each test case starts with a number <strong>N. </strong>After that N positive numbers follow indicating amount of chocolates inside each box. After that an integer <strong>Q</strong> is provided indicating number of queries to be answered. Each query has three integers, A, B and K. The ranges of the variables are described in the description.</p>
<h3>Output</h3>
<p>For each test case, print case number (Check sample output) and then for every query print the number of chocolate box Choco-moo can buy for his K friends from Ath box to Bth box (inclusive) in a newline.</p>
<h3>Example</h3>
<p><strong>Input:</strong></p>
<p>2</p>
<p>5</p>
<p>1 2 3 4 5</p>
<p>2</p>
<p>1 5 1</p>
<p>1 5 2</p>
<p>5</p>
<p>12 32 5 12 9</p>
<p>3</p>
<p>1 5 2</p>
<p>3 5 3</p>
<p>2 5 2</p>
<p><strong>Output:</strong>&nbsp;</p>
<p>Case 1:</p>
<p>5</p>
<p>2</p>
<p>Case 2:</p>
<p>3</p>
<p>2</p>
<p>2</p>
<p>&nbsp;</p>
<p><strong>Explanation</strong>: In Case 1: Query 1 Choco-moo buys all the boxes since all boxes are divisible by 1. In query 2 he buys second and fourth box since they are divisible by 2 ( 2 and 4 ).</p>
<p><strong>Note: </strong>Let me know if you think the judge data is weak or there is ambigutiy/mistake in the problem statment.&nbsp;</p>