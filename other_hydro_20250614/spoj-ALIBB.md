<p>Alibaba the famous character of our childhood stories would like to be immortal in order to keep bringing happiness to children. In order to reach this status he needs to prove that he is still able to do some unusual things. There are <b>n</b> treasures, (<b>n</b> &lt;= 10000) each in a different place located along a straight road. Each treasure has a time limit, after that it vanishes. Alibaba must take all the <b>n</b> treasures, and he must do it quickly. So he needs to figure out the order in which he should take the treasures before their deadlines starting from the most favorable position. Alibaba has the list of places and deadlines of the treasures. A place <b>i</b> is located at distance <b>d<sub>i</sub></b> from the leftmost end of the road. The time it takes to take a treasure is instantaneous.</p>
<p>Alibaba must find <b>the smallest time</b> by which he can take all the treasures.</p>


<h3>Input</h3>
<p>
The first line of the input contains an integer <b>K</b> &lt;= 10 - determining the number of datasets
</p>
<p>Each data set in the input stands for a particular set of treasures. For each set of treasures the input contains the number of treasures, and the list of pairs place - deadline in increasing order of the locations. White spaces can occur freely between the numbers in the input.The input data are correct.</p>

<h3>Output</h3>
<p>For each set of data the program prints the result to the standard output on a separate line. The solution is represented by the smallest time by which Alibaba can take all the treasures before they vanish. If this is not possible then the output is "No solution".</p>

<h3>Example</h3>

<pre><b>Input:</b>
2
5
1 3
3 1
5 8
8 19
10 15
5
1 5
2 1
3 4
4 2
5 3

<b>Output:</b>
11
No solution
</pre>