<p>
A very big corporation is developing its corporate network. At the beginning, each of the <b>N </b>enterprises of the corporation, numbered from 1 to <b>N</b>, organized its own computing and telecommunication center. Soon, for amelioration of the services, the corporation started to collect some enterprises in clusters, each of them served by a single computing and telecommunication center as follows. The corporation chose one of the existing centers <b>I </b>(serving the cluster <b>A</b>) and one of the enterprises <b>J </b>in some other cluster <b>B </b>(not necessarily the center) and linked them with a telecommunication line. The length of the line between the enterprises <b>I </b>and <b>J </b>is |<b>I </b>每 <b>J</b>|(mod 1000). In such a way two old clusters are joined to form a new cluster, served by the center of the old cluster <b>B</b>. Unfortunately after each join the sum of the lengths of the lines linking an enterprise to its serving center could be changed and the end users would like to know what is the new length.</p>
<p>Write a program to keep trace of the changes in the organization of the network that is able at each moment to answer the questions of the users.
</p>

<h3>Input</h3>
<p>
The first line of the input file will contains only the number <b>T </b>of the test cases (1 &lt;= <b>T</b> &lt;= 5). Each test will start with the number <b>N </b>of enterprises (5&lt;=<b>N</b>&lt;=20000). Then some number of lines (no more than 200000) will follow with one of the commands:
</p>
<p>
<b>E I</b>每 asking the length of the path from the enterprise <b>I </b>to its serving center at the moment; <b>I I J </b>每 informing that the serving center <b>I </b>is linked to the enterprise <b>J</b>. The test case finishes with a line containing the word <b>O</b>. There are fewer <b>I </b>commands than <b>N</b> commands.
</p>

<h3>Output</h3>
<p>
The output should contain as many lines as the number of <b>E </b>commands in all test cases. Each line must contain a single number 每 the requested sum of lengths of lines connecting the corresponding enterprise with its serving center. 
</p>

<h3>Example</h3>

<pre><b>Input:</b>
1
4
E 3
I 3 1
E 3
I 1 2
E 3
I 2 4
E 3
O

<b>Output:</b>
0
2
3
5
</pre>