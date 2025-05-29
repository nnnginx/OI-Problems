<p>Discord is in trouble for causing discord, so he is trying to escape from Equestria.
He's arrived at the port, and he doesn't care what boat he gets on, he just wants to get out.
He can see the boat schedule, where he sees that N boats are arriving today,

</p><p>boat 1 arrives any time within a_1 minutes
</p><p>boat 2 arrives any time within a_2 minutes
</p><p>...
</p><p>boat N arrives any time within a_N minutes (uniform distribution)

</p><p>Tell discord the expected number of minutes he needs to wait for a boat to arrive.
</p><p>For some reason, you should be accurate to 10^-6 of a minute.

</p><h3>Input Format:</h3>
<p>T (number of test cases)
</p><p>N1 (number of boats for test case 1)
</p><p>a1 a2 ... aN
</p><p>N2
</p><p>...
</p><p>NT
</p><p>...


</p><h3>Output Format:</h3>
<p>answer1
</p><p>answer2
</p><p>...
</p><p>answerT

</p><h3>Limits:</h3>
<p>1 &lt;= T &lt;= 100
</p><p>1 &lt;= N &lt;= 100
</p><p>1 &lt;= ai &lt;= 1000

</p><p>Also, N * max{ai} &lt;= 10000

</p><pre><b>Sample Input:</b>
4
1
5
3
49 50 51
3
50 50 50
3
2 7 19

<b>Sample Output:</b>

2.500000
12.495000
12.500000
0.874687
(Fixed thanks to <name forgotten="">)
</name></pre>
Note:  Round however Java would round if you used the statement System.out.printf("%.6f\n", answer);