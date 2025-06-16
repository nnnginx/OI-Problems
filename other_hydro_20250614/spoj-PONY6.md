<p>Story:
Twilight Sparkle was working on some formulas when she came across a strange pattern.
</p><p>When she added 1/2 + 1/4 + 1/8 + ..., she saw that it kept getting closer and closer to 1.

</p><p>She was able to figure out that problem and a few more, but there are others that are too difficult.  She needs your help.

</p><h3>Problem Statement</h3>
<p>Given k and r, integers, find
</p><p>Sum from n = 1 to infinity of n^k / r^n.
</p><p>Also you must output the exact value, as a fraction in lowest terms.

</p><h3>Input</h3>
<p>You will be given a number T on the first line.  The following T lines will be of the form
</p><p>S k r
</p><p>where S is a String label with no spaces, and both k and r are as described above.

</p><h3>Output</h3>
<p>Your output will contain T lines of the form
</p><p> S N / D
</p><p> where S is the label you were given in the input, N is the numerator of the answer, and D is the denominator.  D may be 1.
</p><p>To be more precise, if the fraction is negative, then output the negative sign next to N.

</p><h3>Example</h3>

<pre><b>Input:</b>
6
Case1: 0 2
Case2: 0 3
Case3: 0 -3
Label: 2 9
Otherlabel: 12 16
Biggest: 50 -555


<b>Output:</b>
Case1: 1 / 1
Case2: 1 / 2
Case3: -1 / 4
Label: 45 / 256
Otherlabel: 268201436794928 / 320361328125
Biggest: -71542844799237379223056641850683038399677651990786654293842285446351016224553939010
<p>882650681431892067495137019178862799169155069446928707568453465 / 
</p><p>7086055907083154841158073677533359179964732523333455695465110902606507148230087594593
</p><p>20274728690683789654784801111318621847552
</p></pre>
Note: The output for each case should all be on one line.  It is split in the final case here for readability.
<h4>Bounds</h4>
<p>T &lt;= 10000
</p><p>0 &lt;= k &lt;= 50
</p><p>1 &lt; |r| &lt;= 1000
</p><p> The timelimit per case is ~x5 my Java solution.
</p>