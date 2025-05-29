<p>
Lineland is a strange country. As the name suggests, it's shape (as
seen from above) is just a straight line, rather than some
two-dimensional shape.  The landscape along this line is very
mountainous, something which occasionally leads to some problems. One
such problem now occurs: in this modern era the king wants to build an
airport to stimulate the country's economy. Unfortunately, it's
impossible for airplanes to land on steep airstrips, so a horizontal
piece of land is needed. To accommodate for the larger airplanes, this
strip needs to have length at least <em>L</em>.
</p>
<p>
Over the years, the inhabitants of Lineland have become very
proficient in flattening pieces of land. Given a piece a land, they
can remove rock quickly. They don't want to add rock for that may lead
to an unstable landing strip. To minimize the amount of effort,
however, they want to remove the least amount of rock necessary to
reach their goal: a flat piece of land of length <em>L</em>.  What is
this minimum amount?  Because of the low-dimensional nature of
Lineland, the amount of rock that needs to be removed is measured as
the total area of land above the place where the landing strip is
placed, rather than the volume (so in the Figure below, the amount of
land removed is given by the lightly shaded area).
</p>
<p>
<img class="figure" src="/content/overwise:lineland1.png">
</p>
<h3>Input</h3>
<p>
One line with a positive number: the number of test cases (at most 25). Then
for each test case:

</p><ul>

<li>
One line with an integer <em>N</em>, 2 ¡Ü <em>N</em> ¡Ü 500, the
number of points, and an integer <em>L</em>, 1 ¡Ü <em>L</em> ¡Ü

10000, the necessary length to flatten.

</li><li>
<em>N</em> lines with two integers <em>x<sub>i</sub></em> and
<em>y<sub>i</sub></em> with 0 ¡Ü <em>x<sub>i</sub></em>,

<em>y<sub>i</sub></em> ¡Ü 10000 describing the landscape of
Lineland. The <em>x<sub>i</sub></em> are in (strictly) ascending
order. At position <em>x<sub>i</sub></em> the height of the landscape
is <em>x<sub>i</sub></em>. Between two <em>x<sub>i</sub></em> the
landscape has constant slope. (So the landscape is piecewise
linear). The difference between <em>x<sub>N</sub></em> and

<em>x<sub>1</sub></em> is greater than or equal to <em>L</em>.
</li></ul>
<p></p>
<h3>Output</h3>
<p>
For each test case, output one line with the minimum amount of rock
which must be removed in order to build the airport.  The answer
should be given as a floating point number with an absolute error of
at most 10<sup>-3</sup>.
</p>
<h3>Example</h3>

<pre><b>Input:</b>
4
3 5
0 2
4 2
14 0
4 3
0 2
2 0
4 0
5 3
3 10
10 2
30 2
35 7
2 777
222 333
4444 5555

<b>Output:</b>
0.9000
0.3750
0.0000
373362.4867
</pre>