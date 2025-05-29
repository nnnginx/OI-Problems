<p><strong>Fast Delivery Corporation</strong> built one of its offices right in the middle of the longest straight street in Cuba in order to satisfy every order of those customers who live along that street.</p>
<p>The addresses of the houses to which the merchandises are distributed are represented by integer numbers which represent the distance between the office and the corresponding houses. If we consider that the office is located at position 0, then the positive addresses are located to the right of the office, and the negative addresses are located to the left of the office.&nbsp;</p>
<p>The delivery orders are satisfied in the same order in which they were received.</p>
<p>Fast Delivery Corporation has assigned <strong>two </strong>employees to the new office. Those employees are in charge of distributing the merchandises. At the beginning of the day, the orders are shared between both employees.&nbsp;</p>
<p>The corporation wants to share the orders between the two employees in such a way that the total distance required to deliver all the merchandise is <strong>minimized</strong>.</p>
<h3>Input</h3>
<p>Line 1: a single integer N (1 &lt;= N &lt;= 100,000) representing the number of orders</p>
<p>The next N lines contain an integer representing an address where a merchandise will be delivered.</p>
<p>The distance between the office and any house is not greater than 10<sup>8</sup></p>
<h3>Output</h3>
<p>A single line: the minimum distance the two employees have to travel to satisfy every order.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
 5
1
-1
2
-2
3

<strong>Output:</strong>
5</pre>
<pre><strong>Note</strong>: The naive greedy doesn't work. Also remember that the deliveries must be satisfied in the same order they appear in the input.</pre>