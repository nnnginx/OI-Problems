<p>
ACRush and his friends want to open a party to celebrate the good result of THU in ICPC 2007. They will use all halls in THU for their party. There are 2 kinds of hall: the small and the large one. In each hall, there is an electronic light system, which forms a tree topology to reduce redundant wires.

</p><ul type="disc">
<li>In a small hall, the light system is a general tree with n lights. The lights are numbered from 1 to <i>n</i> </li>
<li>In a large hall, the light system is obtained from <i>k</i> chains of lights, each chain has length <i>t</i>. The first lights of these k chains are connected with a big light at the central stage of the hall. The big light has id 1, the first light of each chain has id from 2 to k+1, then we continue with the second light of each chain, so on...</li>
</ul>
<p>
Take a look at the figure below:<br>
<img src="/content/thanhvy:graceful_fig.png">

</p><p>
ACRush hopes in every hall, each light has an unique color and so do the wires!
</p><p>
For easier to remember and to hang up lights against the walls, he sets a
rule:
</p><ul type="disc">
    <li>For each hall, we number the color from 0 to <i>n-1</i>, so each light will get a color id in set {0, 1, ..., <i>n-1</i>}.</li>
    <li>Color id of the wire connects i-th light and j-th light uniquely identified by the positive difference between color ids of i-th light and j-th light.</li>
</ul>
<p>
At first view, the rule seems easy, so everyone agrees with him. But it's really tough if the room is quite large, too hard to set colors for lights.
After few seconds, ACRush says <i>"So in this hall, the 1-st light should have color 3, the 2-nd one should have color 0,..."</i>. Well, how can he do it very fast? <br>

</p><p>
How about you ? Let write a program to help ACRush's friends setting colors for lights in all <i>T</i> halls.

</p><h3>Input</h3>
<p>
The first line of file is <i>T</i> -- number of halls in THU (0 &lt; T &lt;= 10).
The following line is blank. Then, there are the descriptions of T halls. 

</p><p>
For each hall, the first line contains one integer <i>kind</i>. <i>kind</i> denotes which kind of the current hall: 1 is a small hall, 2 is a large one.

On next line, there are two cases:
</p><ul type="disc">
    <li>For Kind 1, first line is n (1 &lt;= n &lt;= 27) -- number of lights. Next <i>n - 1</i> lines describe
wires in this hall. Each line is pair (u, v) -- there is a wire between light u and v (1 &lt;= u, v &lt;= n).</li>
    <li>For Kind 2, only one line contains two numbers k and t (1 &lt;= k, t &lt;= 1000).</li>
</ul>
<p>
There is a blank line after each description.

</p><h3>Output</h3>
<p>
For each hall, show us <i>n</i> numbers on one line, i-th number is the color id of i-th light. If there are many solutions any of them will be accepted. Otherwise, if there is no solution, all color id should be <i>-1</i>.<br>
The color ids on one line are separated by exactly one blank, and you'd better not print any redundant blanks.
There is no blank line after each case.

</p><h3>Example</h3>

<pre><b>Input:</b>
2

1
3
1 2
2 3

2
2 1

<b>Output:</b>
0 2 1
0 4 2 1 3
</pre>