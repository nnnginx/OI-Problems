<p>Egor works as a controller in the bus. Each day he is given a pack of tickets which he then sells. Recently he has become interested about how many tickets in the pack are lucky. He thinks that the more tickets are lucky the luckier day he will have. No he wants to find out how lucky for him will the next day be. The numbers of all tickets consist of n digits. The ticket is considered to be lucky if the sum of the first n/2 digits equals to the sum of the last n/2 digits. Egor knows that the numbers in the pack that he will be given can start with equal probability from any number in the interval from a to b inclusive. The pack holds k tickets. The numbers in the tickets are consecutive. Help Egor find out the expected amount of lucky tickets in the pack.

</p><h3>Input</h3>
<p>The first line of the input file contain number n - the amount of tests. The next n lines consist of three integers a, b §Ú k (0 &lt;= a &lt;= b &lt; 10^12, 1 &lt;= k &lt;= 100000). Integers a, b and b+k consist of the same amount of digits which is equal to the amount of digits in the number of each ticket. They may start with zeroes. The amount of digits in a and b is always even.

</p><h3>Output</h3>
<p>Output the expected quantity of lucky tickets in the pack in the form of irreducible fraction. In case the
result is an integer, no slash should appear in the output.

</p><h3>Example</h3>

<pre><b>Input:</b>
3
0123 4567 150
10 10 20
4000 4999 11

<b>Output:</b>
6519/635
2
103/125

</pre>