<p>There was an application "Guess number!" in one of the popular social network recently. On each of the levels of this offered game it is necessary to define the secret number with some information provided.
</p><p>In particular, one of the most difficult levels consists in  guessing the rational number <i>x</i> (0 &lt; <i>x</i> &lt; 1). It is known, that the result of multiplication of this number by natural number <i>k</i> is exactly one alteration: the <i>i</i>-th and <i>j</i>-th digits after a decimal point are exchanged by each other.
</p><p>As the number in front of decimal point isn't changed, the inequality
0 &lt; <i>kx</i> &lt; 1 is executed. Initially the numbers after a decimal point can be infinite. 
</p><p>Your problem consists in writing the program which will define value <i>x</i> on numbers <i>i</i>, <i>j</i>, <i>k</i>.

</p><h3>Input</h3>
<p>The first input line contains in one integer <i>t</i> (about 1000). Each of the following <i>t</i>  lines contains three numbers: <i>i</i>, <i>j</i>, <i>k</i> (1 ≤ <i>i</i> &lt; <i>j</i> ≤ 1000; 2 ≤ <i>k</i> ≤ 10<sup>9</sup>).

</p><h3>Output</h3>
<p>If the required number exists, output consists in two integers — numerator and denominator of a non-reducible fraction setting required number. Otherwise output is "NO SOLUTION".

</p><h3>Example</h3>

<pre><b>Input:</b>

1
1 4 13

<b>Output:</b>

2997 40000
</pre>