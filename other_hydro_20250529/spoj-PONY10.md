<p>
There is a recently discovered ancient temple, and Daring Do is already exploring it.
She's come across an old Artifact of Power, which just seems to be spouting meaningless numbers. "...82980644837721883829806448..."</p>

<p>Reading the inscription on the wall, it gives an explanation to the artifact:

</p><p style="text-align: center;">WE HAVE TAPPED INTO THE UNIVERSAL LIFE FORCE.</p>
<p style="text-align: center;">WE HEAR THE CLOCK TICKING TOWARD THE END.</p>
<p style="text-align: center;">CAN YOU HEAR IT?</p>
<p style="text-align: center;">WHEN THE PROPHESIED NUMBERS ARE SAID THE FORETOLD NUMBER OF TIMES</p>
<p style="text-align: center;">IT ENDS.</p>

<p>Daring Do doesn't know the prophesied numbers or foretold count, so she moves on with exploring.</p>

<p>She gets more clues while exploring:
</p><ul>
<li>The artifact began counting at the beginning of time, starting from 0 and going up 1 step at a time, saying each digit individually.
So when it first began, it went "0123456789101112131415...".  Each second, it says the next digit. This means at time t=0, it said "0", at time t=1, it said "1", etc.</li>

<li>The universe will end not on the tick after the prophesied number is said for the final time, it ends on the tick that the prophesied number begins. For instance,
if the prophesied numbers were "01", and the foretold number of times were "2", then the universe would end at time t = 11.  See below for more examples.</li>

<li>She's found different things which could be the prophesied numbers, or the foretold number of times, but she's not sure.</li>
</ul>
<p></p>

<p>Please help her figure out the life time of the universe, if the given pair of a 'foretold count' and 'prophesied numbers' were the true ones.
But, if you take too long, the world might end before you figure it out!</p>

<h3>Input Description</h3>
<p>
The first line is an integer T, indicating the number of test cases to follow.
The following T lines will contain 2 things: a number K, the foretold count, and a string composed of digits, TARGET.</p>

<h3>Output Description</h3>
<p>
For each test case, please determine S, the number of seconds until the prophesied number would be said for the final time.
For test case i, please output "Case #i: S" on an individual line.</p>

<h3>Example</h3>

<pre><b>Input:</b>
6
1 0
1 00
9 1
2 01
100 25
5555 178

<b>Output:</b>
Case #1: 0
Case #2: 191
Case #3: 22
Case #4: 11
Case #5: 9018
Case #6: 5104196
</pre>

<h4>Explanation of Case #3</h4>
<p>
The artifact starts "0123456789101112131415<b>1</b>617..."
We see that '1' occurs for the 9th time at time t = 22.</p>

<h3>Limits</h3>
<p>For one test file, T ~= 100000.  For the other five files, T ~= 10000</p>
<p>Of the possibilities found by Daring Do, they all seem to follow this limit:</p>
<p>LEN(K) + LEN(TARGET) &lt;= 17.</p>
<p>In other words, if TARGET = "1", then K could potentially be "9999999999999999", but no larger.</p>
<p>whereas if TARGET = "1234567890123456", then K could potentially be "9", but no larger.</p>