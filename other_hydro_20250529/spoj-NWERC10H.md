<p>In this problem we deal with the calculation of stock prices. You need to know the following things about stock prices:</p>
<ul>
<li>The <em>ask price </em>is the lowest price at which someone is willing to sell a share of a stock.</li>
<li>The&nbsp;<em>bid price </em>is the highest price at which someone is willing to buy a share of a stock.</li>
<li>The <em>stock price</em> is the price at which the last deal was established.</li>
</ul>
<p>Whenever the bid price is greater than or equal to the ask price, a deal is established. A buy order offering the bid price is matched with a sell order demanding the ask price, and shares are exchanged at the rate of the ask price until either the sell order or the buy order (or both) is fulfilled (i.e., the buyer wants no more stocks, or the seller wants to sell no more stocks). You will be given a list of orders (either buy or sell) and you have to calculate, after each order, the current ask price, bid price and stock price.</p>
<h3>Input</h3>
<p>On the first line a positive integer: the number of test cases, at most 100. After that per test case:</p>
<ul>
<li>One line with an integer n (1 ¡Ü n ¡Ü 1&nbsp;000): the number of orders.</li>
<li>n lines of the form "<em>order_type x</em>&nbsp;<tt>shares&nbsp;at y", <span style="font-family: arial, helvetica, sans-serif;">where <em>order_type </em>is either<em> </em>"buy" or "sell", x (1 ¡Ü x ¡Ü 1&nbsp;000) is the number of shares of a stock someone wishes to buy or to sell, and y (1 ¡Ü y ¡Ü 1&nbsp;000) is the desired price.</span></tt></li>
</ul>
<h3>Output</h3>
<p>Per test case:</p>
<ul>
<li>n lines, each of the form "ai bi si" , where ai, bi and si are the current ask, bid and stock prices, respectively, after the i-th order has been processed and all possible deals have taken place. Whenever a price is not defined, output "-" instead of the price.</li>
</ul>
<h3>Example</h3>
<pre><strong>Input:</strong>
<pre>2
6
buy&nbsp;10&nbsp;shares&nbsp;at&nbsp;100
sell&nbsp;1&nbsp;shares&nbsp;at&nbsp;120
sell&nbsp;20&nbsp;shares&nbsp;at&nbsp;110
buy&nbsp;30&nbsp;shares&nbsp;at&nbsp;110
sell&nbsp;10&nbsp;shares&nbsp;at&nbsp;99
buy&nbsp;1&nbsp;shares&nbsp;at&nbsp;120
6
sell&nbsp;10&nbsp;shares&nbsp;at&nbsp;100
buy&nbsp;1&nbsp;shares&nbsp;at&nbsp;80
buy&nbsp;20&nbsp;shares&nbsp;at&nbsp;90
sell&nbsp;30&nbsp;shares&nbsp;at&nbsp;90
buy&nbsp;10&nbsp;shares&nbsp;at&nbsp;101
sell&nbsp;1&nbsp;shares&nbsp;at&nbsp;80</pre>
<strong>Output:</strong>
<pre>-&nbsp;100&nbsp;-
120&nbsp;100&nbsp;-
110&nbsp;100&nbsp;-
120&nbsp;110&nbsp;110
120&nbsp;100&nbsp;99
-&nbsp;100&nbsp;120
100&nbsp;-&nbsp;-
100&nbsp;80&nbsp;-
100&nbsp;90&nbsp;-
90&nbsp;80&nbsp;90
100&nbsp;80&nbsp;90
100&nbsp;-&nbsp;80</pre>
</pre>