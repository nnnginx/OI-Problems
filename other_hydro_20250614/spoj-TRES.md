<p>Lana lives in a small but merry village. There is a row of cherry trees next to the main street. Lana numbered the trees with consecutive integers starting with 1.</p>
<p>After much studying, Lana noticed that the number of the tree uniquely determines the amount of cherries the tree gives.</p>
<p>For one tree, consider consecutive groups of digits in the tree's number. For each group of digits, multiply the digit by the square of the length of the group. Adding these numbers for all groups gives the total number of cherries the tree gives.</p>
<p>For example, in tree number 77744007, the groups are 777, 44, 00 and 7. The amount of cherries will be 7¡¤3^2 + 4¡¤2^2 + 0¡¤2^2 + 7¡¤1^2 = 86 units.</p>
<p>The time has come to pick the cherry trees and the villagers have agreed to pick all trees numbered A through B (inclusive). Write a program that will calculate the total amount of cherries picked.</p>

<h3>Input</h3>
<p>Input consists of two integers A and B (1 ¡Ü A ¡Ü B ¡Ü 10^15), the first and last trees to be picked.</p>

<h3>Output</h3>
<p>Output a single integer, how many units of cherries will be picked.

</p><h3>Example</h3>

<pre><b>Input:</b>
100 111

<b>Output:</b>
68
</pre>