<p>The ponies have finally cornered Discord.  His earlier escape attempts didn't help him much.

</p><p>The unicorn ponies have begun casting magic spells at Discord to turn him back into stone.
There are N ponies and pony I has a casting rate A_I.  That is, once pony I began casting 
her magic spell, it would send a bolt of magic at Discord every A_I seconds, precisely.

</p><p>At time t = 0 seconds, all the ponies began casting their magic.  It has now been M seconds since they began casting.

</p><p>Discord is wearing down.  He only can survive being hit by K-1 more spells before being turned into stone (so the Kth spell will turn him to stone).

</p><p>Determine which pony has the honor of casting the final blow against Discord.

</p><p>Notes:  If multiple ponies send a bolt of magic at the same time, then they hit in order of the smaller rate first.
</p><p>All the ponies are casting different spells, so all the casting rates are distinct.
</p><p>If some ponies cast a bolt of magic after exactly M seconds, that bolt has already hit Discord.  He can survive an additional K-1 spells.

</p><h3>Input</h3>
<p> The input file will begin with a number T on the first line, indicating the number of test cases in the file.  It is followed by 2T lines, which represent the T test cases.  Test case i begins with the label "Case #i: " and is followed by space separated N, M, and K for that case.  On the next line are N space separated integers representing the rates of pony0, pony1, ..., ponyN-1.

</p><pre>T //number of test cases
Case #1: N M K//number of ponies, number of seconds since they began casting, the spell which will turn him to stone
A_0 A_1 ... A_N-1
... (etc.)
</pre>

<h3>Output</h3>
<p>The output contains T lines, one for each test case.  For test case i, begin the line with the label "Case #i: ", and then the index of the pony which has dealt the final blow against Discord.
</p><pre>Case #1: C_1 //C_1 is the pony which casts the final blow against Discord
Case #2: C_2
...
Case #T: C_T </pre>

<h2>Limits</h2>
<pre>Limits:
Number of Test cases varies.  Depends on the instance size.
1 &lt;= N &lt;= 5000
0 &lt;= M &lt;= 10^18 - 1
1 &lt;= K &lt; 2^63 - 1
1 &lt;= A_I &lt;= 10^18
</pre>

<h3>Example</h3>

<pre><b>Input:</b>
5
Case #1: 2 0 4
2 3
Case #2: 2 0 5
2 3
Case #3: 3 7 4
2 3 5
Case #4: 4 55 88
10000 55 3 16
Case #5: 4 9950 23
10000 55 3 16

<b>Output:</b>
Case #1: 0
Case #2: 1
Case #3: 2
Case #4: 2
Case #5: 0
</pre>
<p> 
You can be assured that it will not take more than 10^18 seconds to turn Discord into stone from when the ponies began casting.
</p>