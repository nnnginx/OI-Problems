<p>Farmer John has built a new long barn, with N (2 &lt;= N &lt;= 100,000)
stalls. The stalls are located along a straight line at positions
x1,...,xN (0 &lt;= xi &lt;= 1,000,000,000).<br><br>

His C (2 &lt;= C &lt;= N) cows don't like this barn layout and become
aggressive towards each other once put into a stall. To prevent the
cows from hurting each other, FJ wants to assign the cows to the
stalls, such that the minimum distance between any two of them is
as large as possible.  What is the largest minimum distance?<br>

</p>

<h3>Input</h3>
<p><i>t</i> ¨C the number of test cases, then <i>t</i> test cases follows. <br>
* Line 1: Two space-separated integers: N and C<br>
* Lines 2..N+1: Line i+1 contains an integer stall location, xi<br>
</p>

<h3>Output</h3>
<p>For each test case output one integer: the largest minimum distance.<br>

</p><h3>Example</h3>
<p>
<b>Input:</b>
</p><pre>1
5 3
1
2
8
4
9
</pre>
<p>
<b>Output:</b>
</p><pre>3
</pre>
<p>
<b>Output details:</b>
</p><p>
FJ can put his 3 cows in the stalls at positions 1, 4 and 8, <br>resulting in 
a minimum distance of 3.<br>
</p>