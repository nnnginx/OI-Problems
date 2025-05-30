<p>

The citizens of a small village are tired of being the only inhabitants around without a connection to the Internet. After nominating the future network administrator, his house was connected to the global network. All users that want to have access to the Internet must be connected directly to the admin's house by a single cable (every cable may run underground along streets only, from the admin's house to the user's house). Since the newly appointed administrator wants to have everything under control, he demands that cables of different colors should be used. Moreover, to make troubleshooting easier, he requires that no two cables of the same color go along one stretch of street.
</p><p>
Your goal is to find the minimum number of cable colors that must be used in order to connect every willing person to the Internet.

</p><h3>Input</h3>
<p>
<i>t</i> [the number of test cases, t&lt;=500]<br>
<i>n m k</i> [<i>n</i> &lt;=500 the number of houses (the index of the admin's house is 1)]<br>
      [<i>m</i> the number of streets, <i>k</i> the number of houses to connect]<br>
<i>h</i><sub>1</sub> <i>h</i><sub>2</sub> ... <i>h<sub>k</sub></i> [a list of <i>k</i> houses wanting to be conected to the network, 2&lt;=<i>h<sub>i</sub></i>&lt;=<i>n</i>]<br>
[The next <i>m</i> lines contain pairs of house numbers describing street ends]<br>
<i>e</i><sub>11</sub> <i>e</i><sub>12</sub><br>
<i>e</i><sub>21</sub> <i>e</i><sub>22</sub><br>
...<br>
<i>e</i><sub><i>m</i>1</sub> <i>e</i><sub><i>m</i>2</sub><br>
[next cases]
</p><h3>Output</h3>
<p>
For each test case print the minimal number of cable colors necessary to make all the required connections.

</p><h3>Example</h3>

<pre><b>Input:</b>
2
5 5 4
2 3 4 5
1 2
1 3
2 3
2 4
3 5
8 8 3
4 5 7
1 2
1 8
8 7
1 3
3 6
3 2
2 4
2 5

<b>Output:</b>
2
1
</pre>

<p><img src="/content/cyborg:netadmin.png" alt="Illustration to the first example"></p>
<b>Warning: large Input/Output data, be careful with certain languages</b>