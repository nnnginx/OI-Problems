<p>
<img src="./23858/file/QgcM16cF.png">
</p>
<p>
My birthday is coming up and traditionally I'm serving pie. Not just
one pie, no, I have a number <em>N</em> of them, of various tastes and
of various sizes. <em>F</em> of my friends are coming to my party and
each of them gets a piece of pie. This should be one piece of one pie,
not several small pieces since that looks messy. This piece can be one
whole pie though.
</p>
<p>
My friends are very annoying and if one of them gets a bigger piece
than the others, they start complaining. Therefore all of them should
get equally sized (but not necessarily equally shaped) pieces, even if
this leads to some pie getting spoiled (which is better than spoiling
the party).  Of course, I want a piece of pie for myself too, and that
piece should also be of the same size.
</p>
<p>
What is the largest possible piece size all of us can get?  All the
pies are cylindrical in shape and they all have the same height 1,
but the radii of the pies can be different.
</p>
<h3>Input</h3>
<p>
One line with a positive integer: the number of test cases. Then
for each test case:
</p><ul>
<li>
One line with two integers <em>N</em> and <em>F</em> with 1 ��
<em>N, F</em> �� 10000: the number of pies and the number of
friends.

</li><li>
One line with <em>N</em> integers <em>r<sub>i</sub></em> with 1 ��
<em>r<sub>i</sub></em> �� 10000: the radii of the pies.
</li></ul>
<p></p>
<h3>Output</h3>
<p>
For each test case, output one line with the largest possible volume
<em>V</em> such that me and my friends can all get a pie piece of size
<em>V</em>.  The answer should be given as a floating point number
with an absolute error of at most 10<sup>-3</sup>.
</p>
<h3>Example</h3>

<pre><b>Input:</b>
3
3 3
4 3 3
1 24
5
10 5
1 4 2 3 4 5 6 5 4 2

<b>Output:</b>
25.1327
3.1416
50.2655
</pre>