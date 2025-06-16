<p>Byteasar has a cottage. Lately, he has bought n trees and had them planted all in one row. Byteasar does not,
however, like the order which the trees have been planted in. It particularly annoys him that tall and short
ones have been mixed up, and the composition does not meet his aesthetic criteria.
</p><p>Byteasar has invented a <i>disorder coefficient</i> so as to allow the gardener to comprehend his intentions: the
lower the value of the coefficient the prettier the row of trees. It is defined in the following way: |h<sub>1</sub>−h<sub>2</sub>|+
|h<sub>2</sub>−h<sub>3</sub>|+...+|h<sub>n−1</sub>−h<sub>n</sub>|, where h<sub>1</sub>,h<sub>2</sub>, . . . ,h<sub>n</sub> are the heights of consecutive trees in a row.
</p><p>Replanting is a very toilsome and cumbersome task, therefore Byteasar has ordered the gardener to replant
two trees at the most (i.e. interchange their positions). The task of the gardener is to choose the pair to replant
in a way that makes the disorder coefficient the smallest.
</p><p>The gardener is not sure if he has chosen the correct pair of trees and he fears he may lose his job if
he is mistaken. Help him: for each tree calculate the minimal disorder coefficient that may be attained by
switching places with any other tree.

</p><h3>Task</h3>
<p>Write a program which:
</p><ul>
<li> reads the height of the consecutive trees in a row from the standard input,
</li><li> for each tree calculates the minimal disorder coefficient that may be attained should it switch places
with some other tree (or should there be no change at all),
</li><li> writes the outcome to the standard output.
</li></ul>

<h3>Input</h3>
<p>The first line of the standard input contains one integer <i>n</i> (2 &lt;= <i>n</i> &lt;= 50000). The other contains <i>n</i> integers h<sub>i</sub>
(1 &lt;= h<sub>i</sub> &lt;= 100000000) separated by single spaces, denoting the height of the consecutive trees in the row.

</p><h3>Output</h3>
<p>The output should consist of precisely <i>n</i> lines. The i-th line should contain a single integer - the smallest
disorder coefficient attainable when considering replanting of the i-th tree.

</p><h3>Example</h3>

<pre><b>Input:</b>
5
7 4 5 2 5

<b>Output:</b>
7
7
8
7
7
</pre>
<b>* Added some unofficial tests</b>