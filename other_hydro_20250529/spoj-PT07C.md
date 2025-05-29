<p>
    Jiajia is the king of the GbAaY Kingdom. He always squeezes his 20 ministers as coolies.
    There are <i>n</i> cities and <i>m</i> two-way roads connecting cities in the kingdom.
    Because of the increasing of the oil fee, he want to simplify the road system
    in the GbAaY Kingdom to save the traffic cost.
    Thus, some of roads will be removed. But he requests the ministers guarantee
    that there is always a path between any two cities.
    GbAaY Minister Loner suggests Jiajia for the convenience of the traffic management,
    the farthest distance between cities should be minimal. Unhesitatingly, Jiajia agrees this resolution.
    As the GbAaY Kingdom's minister (cooly), you must work hard for Jiajia to make the simplification plan.
</p>

<h3>Input</h3>
<p>   The first line contains two integers <i>n</i>, <i>m</i> (1 &lt;= <i>n</i> &lt;= 200, <i>n</i> - 1 &lt;= <i>m</i> &lt;= 20000).
    Each line of the following <i>m</i> lines contains three integers <i>u</i>, <i>v</i>, <i>w</i> (<i>u</i> != <i>v</i>, 0 &lt;= <i>w</i> &lt;= 10<sup>5</sup>).
    They denote there is a road with length <i>w</i> between city <i>u</i> and city <i>v</i>.
</p>

<h3>Output</h3>
<p>The first line contains one integer which is the farthest distance between cities after the simplification.
    Each line of the follow <i>n</i> - 1 contains two integers <i>u</i>, <i>v</i> (<i>u</i> &lt; <i>v</i>).
    They denote there is an road between city <i>u</i> and city <i>v</i> in the simplification plan.
    If there are many optimal solutions, any of them will be accepted.</p>

<h3>Example</h3>

<pre><b>Input:</b>
3 3
1 2 1
2 3 1
1 3 1

<b>Output:</b>
2
1 2
1 3

</pre>