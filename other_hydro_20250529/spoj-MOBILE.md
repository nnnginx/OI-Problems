<p>Mobile<br>
Manfred loves to build mobiles out of old CDs. For each one, he has an exact plan how it should look like: The CDs are all hanging exactly on the same height. For each pair
of CDs, he writes down the height of the lowest bar such that both CDs are hanging somewhere under this bar. For example, the following mobile and distance matrix fit together:</p><p>
<br>
<img src="/ADB_67/content/mobile.png"></p><p>
<br>
After a while, Manfred realizes that he does not succeed to build every mobile he planned to. For example, there is no solution for the following distance matrix:<br>
     0 1 2<br>
     1 0 3<br>
     2 3 0<br>
So, he decides to write a computer program that checks the distance matrices and tells him if there is a solution.

</p><h3>Input</h3>
<p>Several matrices to check. The first row contains the size of the matrix N (N &lt;= 2048), the next N rows contain the distances in the matrix. Then, the data of the next matrix comes, and so on. All distances are positive integers smaller than 2048. The input is terminated by a zero as matrix size.

</p><h3>Output</h3>
<p>For each matrix, write true if Manfred can build a mobile, false otherwise.

</p><h3>Example</h3>

<pre><b>Input:</b>
5
0 1 1 1 3
1 0 1 1 3
1 1 0 1 3
1 1 1 0 3
3 3 3 3 0
3
0 1 2
1 0 3
2 3 0
3
1 1 1
1 0 2
1 1 0
0

<b>Output:</b>
true
false
false

</pre>