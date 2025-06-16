<p>
"ABEAS Corp." is a very small company that owns a single airplane. The
customers of ABEAS Corp are large airline companies which rent the
airplane to accommodate occasional overcapacity.</p>

<p>Customers send renting orders that consist of a time interval and a
price that the customer is ready to pay for renting the airplane during
the given time period.

Orders of all the customers are known in advance. Of course, not all
orders can be accommodated and some orders have to be declined. Eugene
LAWLER, the Chief Scientific Officer of ABEAS Corp would like to
maximize the profit of the company.</p>

<p>You are requested to compute an optimal solution.
</p>

<h4>Small Example</h4>
<p>
Consider for instance the case where the company has 4 orders:</p>
<ul>
<li>Order 1 (start time 0, duration 5, price 10)</li>
<li>Order 2 (start time 3, duration 7, price 8)</li>
<li>Order 3 (start time 5, duration 9, price 7)</li>
<li>Order 4 (start time 6, duration 9, price 8)</li>
</ul>
<p>
The optimal solution consists in declining Order 2 and 3 and the gain
is 10+8 = 18.<br>
Note that the solution made of Order 1 and 3 is feasible (the airplane
is rented with no interruption from time 0 to time 14) but non-optimal.
</p>

<h3>Input</h3>
<p>
The first line of the input contains a number T ¡Ü 30 that indicates the number of test cases to follow. The first line of each test case contains the number of orders n (n ¡Ü 10000). In the following n lines the orders are given. Each order is described by 3 integer values: The start time of the order st (0 ¡Ü st &lt; 1000000), the duration d of the order (0 &lt; d &lt; 1000000), and the price p (0 &lt; p &lt; 100000) the customer is ready to pay for this order.
</p>

<h3>Output</h3>
<p align="justify">
You are required to compute an optimal solution. For each test case your program has to write the total price paid by the airlines.
</p>
<h3>Example</h3>
<pre><b>Input:</b>
1
4
0 5 10
3 7 14
5 9 7
6 9 8

<b>Output:</b>
18
</pre>
<b>Warning: large Input/Output data, be careful with certain languages</b>