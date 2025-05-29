<p>Harish went to a supermarket to buy exactly ¡®k¡¯ kilograms apples for his ¡®n¡¯ friends. The supermarket was really weird. The pricing of items was very different. He went to the Apples section and enquired about the prices. The salesman gave him a card in which he found that the prices of apples were not per kg. The apples were packed into covers, each containing ¡®x¡¯ kg of apples, x &gt; 0 and ¡®x¡¯ is an integer. An ¡®x¡¯ kg packet would be valued at ¡®y¡¯ rupees. So, the placard contained a table with an entry ¡®y¡¯ denoting the price of an ¡®x¡¯ kg packet. If ¡®y¡¯ is -1 it means that the corresponding packet is not available. Now as apples are available only in packets, he decides to buy atmost ¡®n¡¯ packets for his ¡®n¡¯ friends i.e he will not buy more than n packets of apples.</p>

<p>Harish likes his friends a lot and so he does not want to disappoint his friends. So now, he will tell you how many friends he has and you have to tell him the minimum amount of money he has to spend for his friends.</p>

<h3>Input</h3>
<p>The first line of input will contain the number of test cases, C.</p>
<p>Each test case will contain two lines.</p>
<p>The first line containing N and K, the number of friends he has and the amount of Apples in kilograms which he should buy.</p>
<p>The second line contains K space separated integers in which the ith integer specifies the price of a ¡®i¡¯kg apple packet. A value of -1 denotes that the corresponding packet is unavailable.</p>
<ul>
  <li>0 &lt; N &lt;= 100</li>
  <li>0 &lt; K &lt;= 100</li>
  <li>0 &lt; price &lt;= 1000</li>
</ul>

<h3>Output</h3>
<p>The output for each test case should be a single line containing the minimum amount of money he has to spend for his friends. Print -1 if it is not possible for him to satisfy his friends.</p>

<h3>Sample I/O</h3>
<pre><strong>Input:</strong>
2
3 5
-1 -1 4 5 -1
5 5
1 2 3 4 5

<strong>Output:</strong>
-1
5</pre>

<p><strong>Explanation of test cases:</strong></p>
<p>1) As there are only 3 and 4kg packets in the shop, he will not be able to satisfy his friends as he would not be able to buy exactly 5kg of apples.</p>
<p>2) He can buy five 1kg packet as he has to buy 5 kg. So the min money he should spend is 5.</p>