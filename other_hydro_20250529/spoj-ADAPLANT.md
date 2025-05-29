<p>Ada the Ladybug has grown many plants. She was trying to grow all plants
with equal size. Now she is wondering about the biggest difference between
heights of two plants which are near each other. Plants are near each other, if there are at most <b>K</b> plants between them.</p>


<h3>Input</h3>
The first line contains <b>T</b>, the number of test-cases.

The first line of each test-case will contain <b>N, K</b>, <b>1 &lt; N ¡Ü
    10<sup>5</sup> </b>,<b>0 ¡Ü K ¡Ü
    10<sup>5</sup> </b> where <b>N</b> indicates number of plants.

<p>Next line will contain <b>N</b> integers <b>0 ¡Ü h<sub>i</sub> ¡Ü
    10<sup>9</sup></b> indicating height
of i-th plant.

</p><p>Sum of all <b>N</b> among all test-cases won't exceed <b>3*10<sup>6<sup></sup></sup></b>

</p><h3>Output</h3>
For each test-case, print exactly one number - the biggest difference of plants
near each other (biggest <b>h<sub>i</sub>-h<sub>j</sub></b> such that
<b>|i-j|-1 ¡Ü K</b>).
<h3>Example Input</h3>
<pre>3
5 0
1 2 3 5 6
4 6
1 10 2 9
10 1
1 7 8 9 19 11 21 8 11 0 
</pre>
<h3>Example Output</h3>
<pre>2
9
13
</pre>