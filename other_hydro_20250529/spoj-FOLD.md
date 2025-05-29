<p>

Read the statement of problem E: Edge to understand how to fold a sheet of paper and how to interpret the input.
We define a "stripe" to be a maximally large part of the sheet that has no folding line going through.
Since the turns occur at equidistant places, all stripes are congruent.

</p><p>

In this problem you are given the description of the result of performing several folding steps as in problem E: Edge, i.e., in the unfolded state.
Additionally, you know that the length of the sheet in its folded state is exactly the length of 1 stripe (again, we ignore thickness).

</p><p>

Find the minimum number of folding steps necessary to generate the described sheet from an initially flat sheet of paper.
Note that performing a folding step may create more than one turn in the result because parts of the sheet already overlay due to previous folding steps.
When a step is carried out, however, all overlaying parts of the sheet are affected, i.e., it is not allowed to fold, say, only the top three layers.

</p><p>

Finally, note that every result can be obtained by iterating through the turns in a fixed direction and performing a folding step at each turn, thereby accumulating a 1 stripe long stack of all stripes.
If <code>n</code> is the number of turns in the input description, this procedure in fact requires <code>n</code> folding steps, which is not necessarily minimal as can be observed in the sample output.


</p><h3>Input Specification</h3><p>

The input contains several test cases, each on a separate line.
Each line contains a nonempty string of characters <tt>A</tt> and <tt>V</tt> describing the longer edge of the sheet.
You may assume that the length of the string is less than 200.
The input file terminates immediately after the last test case.

</p><h3>Output Specification</h3><p>

For each test case print on a line the minimum number of folding steps required to produce the described sheet of paper.

</p><h3>Sample Input</h3><p>

</p><pre>V
AVV
AAVAAVVVAAV
</pre>

<h3>Sample Output</h3><p>

</p><pre>1
2
4
</pre>