<p>A beehive is an enclosed structure in which some honey bee species live and raise their<br>young. In this problem we consider a two-dimensional sketch of the beehives. Each<br>beehive is composed of a certain number of cells, where each cell is a regular hexagon.<br>Each cell may have some neighbors, which are other cells that share a side with that cell.<br>A cell with exactly 6 neighbors is an internal cell, while a cell with fewer neighbors is an<br>external one. Notice that an external cell can always be changed to internal by adding<br>some neighbor cells.</p>
<p><br>We are interested in a particular class of beehives. This class of valid beehives is defined<br>recursively as follows: a) a single cell is a valid beehive; and b) given a valid beehive B,<br>if we add the minimum number of cells such that each external cell of B becomes an<br>internal cell, the result is a valid beehive.</p>
<p>The number of cells in a valid beehive is called a beehive number. Given an integer N ,<br>you must decide whether it is a beehive number.</p>
<h3>Input</h3>
<p>Each test case is described using a single line. The line contains an integer N (1 ≤ N ≤<br>10<sup>9</sup> ). The end of input is indicated with a line containing a single −1.</p>

<h3>Output</h3>
<p>For each test case, output a single line containing an uppercase “Y” if N is a beehive<br>number, or an uppercase “N” otherwise.</p>

<h3>Example</h3>

<pre><strong>Input:</strong><br>43<br>1<br>7<br>19<br>15<br>-1<br>
<strong>Output:</strong><br>N<br>Y<br>Y<br>Y<br>N</pre>