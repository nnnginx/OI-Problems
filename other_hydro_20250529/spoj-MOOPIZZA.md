<p>
Moo U's cafeteria has run out of hay and so must order pizzas for
the C (1 &lt;= C &lt;= 1,000) calves attending Moo U.  Conveniently, a
large pizza from the local pizzeria, Pizza Farm, serves exactly one
calf.
</p>
<p>
Pizza Farm is willing to make a pizza for each calf, but, due to
the size of the order, has three constraints on the order:</p>
<p>
   * Although Pizza Farm has long list of T (1 &lt;= T &lt;= 30) vegetarian
     toppings, each of the pizzas must have exactly K (1 &lt;= K &lt;=
     T) toppings<br><br>
   * No topping on a pizza can be duplicated (a pizza cannot have
     onions and onions, for example).<br><br>
   * No two pizzas in the order can have the same set of toppings.<br><br>
     For example, if pizza 1 has onions, green peppers, pineapples,
     and wheat grass, then it can be the only pizza with that exact
     set of toppings, although pizza 2 might have onions, green
     peppers, pineapples, and also olives.<br></p>
<p>
For ordering purposes, the toppings are numbered 1..T.</p>
<p>
The calves at Moo U are very picky when it comes to their pizza
toppings.  Some calves might not like all of the toppings available.
A calf will eat a pizza only she likes every single one of the
toppings on that pizza.  Determine the maximum number of calves
that can be fed.</p>
<h3>Input</h3>
<p>
* Line 1: Three integers: C, T, and K.

* Lines 2..C+1: Each line of space-separated integers describes which
        toppings one of the calves likes.  The first integer on a line
        is the number of topping the calf likes.  The remaining
        integers on the line are the toppings that the calf likes.
</p><h3>Output</h3>
<p>

* Line 1: A single integer, the maximum number of calves that can be
        fed.</p><h3>Example</h3>

<pre><b>Input:</b>

3 2 1
2 2 1
1 1
1 2

</pre>

<b>Input details:</b>
<p>
There are three calves.  Pizza Farm has two toppings and each pizza
must have exactly one topping.  The first calf likes both of the
toppings, the second calf likes only the first topping, and the
third calf likes only the second topping.
</p>
<pre><b>Output:</b>

2
</pre>
<b>Output details:</b>
<p>
There are only two pizzas that can be made: a pizza with topping 1 and a
pizza with topping 2.  If the first pizza is given to the first
calf (since she likes topping 1) and the second pizza to the third calf
(since she likes topping 2), two calves will be fed.  There is no way to
feed
all three calves.</p>