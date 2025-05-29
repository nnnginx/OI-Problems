<p>
Bob loves Pizza but is always out of money. One day he reads in the newspapers that his favorite pizza restaurant,
Alfredo's Pizza Restaurant, is running a competition: they will donate a big pizza to the first person who will tell
them the lowest price per area that can be achieved by buying any of the pizzas at most once. "That task is easy!",
thinks Bob, "For each pizza I just calculate the average price and the lowest quotient will be the answer.".
</p>
<p>
Unfortunately the problem is a bit more complicated: with some pizzas Alberto gives out discount coupons for getting
another pizza cheaper and even worse, those coupons can be combined. The pizzas have to be bought one after the other,
and it is not possible to use a coupon to get a discount retrospectively for a pizza which has already been bought.
Can you help Bob to become the first to solve this task and to get a pizza for free?
</p>

<h3>Input</h3>
<p>
The input file contains several test cases. Each test case starts with a number <i>m</i>, the number of pizzas
Alfredo offers. Input is terminated by <i>m=0</i>. Otherwise, <i>1 ¡Ü m ¡Ü 15</i>. Then follow <i>m</i>

lines describing the pizzas. Each of those following lines describes pizza <i>i</i> (<i>1 ¡Ü i ¡Ü m</i>)
and starts with 3 integer numbers <i>p<sub>i</sub></i>, <i>a<sub>i</sub></i> and <i>n<sub>i</sub></i> specifying
the price of the pizza, its area and the number of discount coupons you get when buying it,

<i>1 ¡Ü p<sub>i</sub> ¡Ü 10000</i>, <i>1 ¡Ü a<sub>i</sub> ¡Ü 10000</i> and <i>0 ¡Ü n<sub>i</sub> &lt; m</i>.
Then follow <i>n<sub>i</sub></i> pairs of integer numbers <i>x<sub>i,j</sub></i> and <i>y<sub>i,j</sub></i> specifying
the index <i>x<sub>i,j</sub></i> (<i>1 ¡Ü x<sub>i,j</sub> ¡Ü m, x<sub>i,j</sub> ¡Ù i</i>) of the pizza you get a
discount coupon for and the discount in percentage terms <i>y<sub>i,j</sub></i> (<i>1 ¡Ü y<sub>i,j</sub> ¡Ü 50</i>)
you get when buying pizza <i>x<sub>i,j</sub></i>.
You may assume that for each <i>i</i> the values <i>x<sub>i,j</sub></i> are pairwise distinct.

</p>

<h3>Output</h3>
<p>
For each test case print one line containing the lowest price per area that can be achieved by buying any of the pizzas
at most once. Round this number to 4 places after the decimal point. Note that you can combine an arbitrary number of
discount coupons: for a pizza with price 10 and two rabatt coupons for that pizza with a 50 and a 20 on it, you would
only have to pay 10 * 0.8 * 0.5 = 4 monetary units.
</p>

<h3>Example</h3>

<pre><b>Input:</b>
1
80 30 0
2
200 100 1 2 50
200 100 0
5
100 100 2 3 50 2 50
100 100 1 4 50
100 100 1 2 40
600 600 1 5 10
1000 10 1 1 50
0
<b>Output:</b>
2.6667
1.5000
0.5333
</pre>