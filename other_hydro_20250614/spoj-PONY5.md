<p>Since the Iron Pony competition was such fun last year, the ponies have decided to host a similar event this year, but this time it would be in teams.  When each pony arrives at the event, they receive a number between 1 and 10^18.  It is possible that some ponies receive the same number.  Once everypony arrives, Miss Mayor will announce a number X and how to determine which team a pony is on - the pony takes their given number and looks at the result modulo X.  That is their team number.

</p><p>Dr. Whooves is at the event with a group, and he was wondering about the numbers X that would let his entire group be on the same team.  Dr. Whooves likes big numbers, so he is going to suggest to Miss Mayor the number X which is the largest number that would let his entire group be on the same team.

</p><p>Your goal is to determine what number Dr. Whooves suggested to Miss Mayor.
But because the number might be really big, if there is a valid X larger than 10^18, just print "I can't count that high".

</p><h3>Input</h3>
<p>The input will contain one line with a number T, the number of test cases in the file.
</p><p>On the next T lines, one for each of the cases. The format of the case is "Case #i: N a1 a2 ... aN" where N is the number of ponies in Dr. Whooves's group, and each a_j is the number given to a pony in his group.

</p><h3>Output</h3>
<p>There will be T lines in your output, one for each of the test cases in the input.  The output format for case i is "Case #i: X" where X is the number that Dr. Whooves suggests to Miss Mayor, unless X is too large, and then you print "I can't count that high" [see sample output]

</p><h3>Example</h3>

<pre><b>Input:</b>
2
Case #1: 3 178 928 440
Case #2: 1 1000000000000000000

<b>Output:</b>
Case #1: 2
Case #2: I can't count that high
</pre>

<h4>Limits</h4>
1 &lt;= N &lt;= 1000000 (10^6)

<h5>Warning: Large input files</h5>