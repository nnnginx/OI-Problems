<p>As the result of the gas wars the following agreement was made. The transit of the gas was allowed under the following conditions. There are <b>n</b> transit nodes and <b>m</b> pipes connecting those nodes. There <b>k</b> nodes where the gas enters and <b>l</b> nodes where it should be moved. Each pipe has a carrying capacity of <b>c<sub>i</sub></b> cubic meters of gas per day. Gas can go through the pipes in either direction. It is needed to move <b>g</b> cubic meters of gas in total through the pipeline every day. The cost of the transit is defined as <b>maxC</b>*100 thousand dollars, where <b>maxC</b> 每 maximum of carrying capacities of the used in the transit pipes (even those which are not fully used). You are to find the minimum possible cost of transit for the given pipeline.

</p><h3>Input</h3>
<p>The first line of the input file contains <b>t</b> 每 the amount of test cases. The description of each test case follows. The first line of each test case contains five integers separated by spaces 每 <b>n</b>, <b>m</b>, <b>k</b>, <b>l</b>, <b>g</b>. Then <b>m</b> lines containing three integers <b>a</b>, <b>b</b>, <b>c</b> follow. Each lines means that nodes with numbers <b>a</b> and <b>b</b> are connected by the pipe with the carrying capacity of <b>c</b>. Next line contains <b>k</b> integers 每 the numbers of nodes where the gas should enter the pipeline. The last line of the test case contains <b>l</b> integers 每 the numbers of nodes where the gas should be moved. The gas can enter the pipeline in any of the <b>k</b> entrance nodes and can be moved to any of the <b>l</b> exit nodes. The nodes are numbered from 1 to <b>n</b>.

</p><h3>Constraints</h3>
<p>1 &lt;= <b>t</b> &lt;= 20<br>
2 &lt;= <b>n</b> &lt;= 100<br>
1 &lt;= <b>m</b> &lt;= <b>n</b>*(<b>n</b>-1)/2<br>
1 &lt;= <b>k</b>, <b>l</b> &lt;= <b>n</b>/2<br>
1 &lt;= <b>g</b>, <b>c</b> &lt;= 1000000<br>

</p><h3>Output</h3>
<p>For each test case output a single integer on a separate line 每 the minimum cost of transit in thousands of dollars. If the transit of the needed volume is impossible, then output -1.

</p><h3>Example</h3>

<pre><b>Input:</b>
1
6 8 1 1 1
1 2 1
1 3 2
2 4 3
2 5 3
3 4 4
3 5 2
4 6 4
5 6 1
1
6

<b>Output:</b>
200
</pre>