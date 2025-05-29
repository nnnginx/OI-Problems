<p>There are some friends living in a hostel who share many things among them daily. They are very economical and never want to waste a penny. Whenever they need something which they can share among them to save money, they do. But the real problem is: whenever they buy some item which they'll share among them, it's very difficult to share the price of the item among them instantly e.g. some item costs 10 bucks and to be shared among 3 friends, each friend gets a share of 3.33 bucks to pay, it's difficult to share it instantly, isn't it? I mean all of them may not have exactly 3.33 bucks in their wallet to pay for settlement. Assume they always pay in cash and share the price of the item equally among them.</p>
<p>So, all the friends come up with below idea to ease their lives:</p>
<p><strong>"Every time we buy some item which is going to be shared among some or all of us, we need not share its price while buying it. Instead one or some of us will pay it while buying and record it for settlement at the end of month."</strong></p>
<p>Basically, they need a software application where <em>"they can record the purchase of a shared item with its name, purchase date, price, who paid how much while buying it and among whom the item is going to be shared. At the end of the month, the application should be able to find out, who owes how much to whom."</em></p>
<p>So far, so good.&nbsp;But...</p>
<ol>
<li>At the end of the month, the application should find out the minimum number of transactions needed among friends for settlement. Say, A needs to pay 10 bucks to B (A-&gt;B: 10) and B needs to pay 5 bucks to A (B-&gt;A: 5), then A can just pay 5 bucks to B (A-&gt;B: 5) and so only 1 transaction is enough for settlement. Similarly, if A-&gt;B: 10 and B-&gt;C: 10, then A-&gt;C: 10 (only 1 transaction is enough again).</li>
<li>Sum of the amounts in all transactions in final settlement should be minimum. Say, A-&gt;B: 10 and B-&gt;C: 5 (sum of the amounts = 10+5 = 15), then A-&gt;B: 5 and A-&gt;C: 5 (sum of the amounts = 5+5 = 10) should be the transactions in final settlement.</li>
</ol>
<h3>Input</h3>
<ul>
<li>First line of Input will contain the number of test cases <strong>T (1 &lt;= T &lt;= 100)</strong>. <strong>T</strong> test cases follow.</li>
<li>First line of each test case will contain two integers <strong>N</strong> and <strong>S</strong>, the number of friends <strong>N (1 &lt;= N &lt;= 100) </strong>numbered from 1 to N and the number of transactions <strong>S (1 &lt;= S &lt;= 1000)</strong> amongst friends within a month.</li>
<li><strong>2<sup>nd</sup> to (S+1)<sup>th</sup></strong> lines of each test case will contain the descriptions of all <strong>S</strong> transactions, one transaction per line in this format (all values are space separated, angular brackets are for clarification only): <strong>&lt;F&gt; &lt;A&gt; &lt;B<sub>1</sub>&gt; &lt;B<sub>2</sub>&gt; ... &lt;B<sub>N</sub>&gt;</strong> where                              
<ul>
<li><strong>F (1&lt;= F &lt;= N): </strong>serial number of a friend,&nbsp;</li>
<li><strong>A (0.01 &lt;= A &lt;= 10000.00): </strong>amount with 2 decimal places paid by <strong>F</strong> in this transaction and&nbsp;</li>
<li><strong>B<sub>i</sub> (0 or 1):</strong>&nbsp;0 if the amount <strong>A</strong> is not to be shared with friend numbered <strong>i</strong>, 1 if it is to be shared with friend numbered <strong>i</strong>. Amount is shared with at least one of the friends. <em>(Note: if amount <strong>A</strong> is to be shared among <strong>n</strong> friends, truncate each share i.e. <strong>A/n</strong>&nbsp;to 2 decimal places. e.g. if A=10.00 and n=3, then A/n=3.33, similarly if A=20.00 and n=3, then A/n=6.66)</em></li>
</ul>
</li>
</ul>
<h3>Output</h3>
<p>For each test case, find a solution with minimum number of transactions in final settlement, with sum of the amounts involved in those transactions being minimum (call it <strong>MINIMUM_SUM_AMOUNTS</strong>).</p>
<ul>
<li>Output a single line for each test case containing the <strong>MINIMUM_SUM_AMOUNTS </strong>with 2 decimal places only.</li>
</ul>
<h3>Example</h3>
<p><strong>Input:</strong></p>
<pre>2
2 2
1 5.00 0 1
2 10.00 1 0
3 2
2 10.00 1 0 0
3 5.00 0 1 0
</pre>
<p><strong>Output:</strong></p>
<pre>5.00
10.00
</pre>
<p><strong>Explanation:</strong></p>
<pre>1. For 1st testcase, friend #1 will pay 5.00 bucks to friend #2 in the final settlement. (MINIMUM_SUM_AMOUNTS = 5.00)
2. For 2nd testcase, friend #1 will pay 5.00 bucks each to friend #2 and friend #3 in the final settlement. (MINIMUM_SUM_AMOUNTS = 5.00 + 5.00 = 10.00)
</pre>