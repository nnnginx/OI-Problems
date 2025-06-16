<p>

For hundreds of years Fermat's Last Theorem, which stated simply that
for <i>n</i> &gt; 2 there exist no integers <i>a</i>, <i>b</i>, <i>c</i>
&gt; 1 such that <i>a</i>^<i>n</i> = <i>b</i>^<i>n</i> +
<i>c</i>^<i>n</i>, has remained elusively unproven.  (A recent proof
is believed to be correct, though it is still undergoing scrutiny.)
It <i>is</i> possible, however, to find integers greater than 1 that
satisfy the "perfect cube" equation <i>a</i>^3 = <i>b</i>^3 +
<i>c</i>^3 + <i>d</i>^3 (e.g. a quick calculation will show that the
equation 12^3 = 6^3 + 8^3 + 10^3 is indeed true).  This problem
requires that you write a program to find all sets of numbers
{<i>a</i>,<i>b</i>,<i>c</i>,<i>d</i>} which satisfy this equation for
<i>a</i> &lt;= 100. </p><p>

The output should be listed as shown below, one perfect cube per line,
in non-decreasing order of a (i.e. the lines should be sorted by their
<i>a</i> values).  The values of <i>b</i>, <i>c</i>, and <i>d</i>
should also be listed in non-decreasing order on the line itself.
There do exist several values of <i>a</i> which can be produced from
multiple distinct sets of <i>b</i>, <i>c</i>, and <i>d</i> triples.
In these cases, the triples with the smaller <i>b</i> values should be
listed first.  </p><p>

Note that the programmer will need to be concerned with an efficient
implementation.  The official time limit for this problem is 2
minutes, and it is indeed possible to write a solution to this
problem which executes in under 2 minutes on a 33 MHz 80386 machine.
Due to the distributed nature of the contest in this region, judges
have been instructed to make the official time limit at their site the
greater of 2 minutes or twice the time taken by the judge's solution
on the machine being used to judge this problem. </p><p>

The first part of the output is shown here: </p><p>

</p><pre>Cube = 6, Triple = (3,4,5)
Cube = 12, Triple = (6,8,10)
Cube = 18, Triple = (2,12,16)
Cube = 18, Triple = (9,12,15)
Cube = 19, Triple = (3,10,18)
Cube = 20, Triple = (7,14,17)
Cube = 24, Triple = (12,16,20)
</pre>