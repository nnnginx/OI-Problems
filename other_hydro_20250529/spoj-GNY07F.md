<p>Deep in the Amazon jungle, exceptionally tall trees grow that support a rich biosphere of figs and
juniper bugs, which happen to be the culinary delight of brown monkeys.

</p><p>Reaching the canopy of these trees requires the monkeys to perform careful navigation through the
tall tree¡¯s fragile vine system. These vines operate like a see-saw: an unbalancing of weight at any
vine junction would snap the vine from the tree, and the monkeys would plummet to the ground
below. The monkeys have figured out that if they work together to keep the vines properly balanced,
they can <i>all</i> feast on the figs and juniper bugs in the canopy of the trees.

</p><p>A <i>vine junction</i> supports exactly two <i>sub-vines</i>, each of which must contain the same number of
monkeys, or else the vine will break, leaving a pile of dead monkeys on the jungle ground. For
purposes of this problem, a <i>vine junction</i> is denoted by a pair of matching square brackets [ ], which
may contain nested information about junctions further down its <i>sub-vines</i>. The nesting of vines will
go no further than <b>25</b> levels deep.

</p><p><img align="center" src="./22612/file/zdXKzPWk.png">

</p><p>You will write a program that calculates the <i>minimum</i> number of monkeys required to balance a
particular vine configuration. There is <b>always</b> at least one monkey needed, and, multiple monkeys
may hang from the same vine.

</p><h3>Input</h3>
<p>The first line of input contains a single integer N, (1 ¡Ü N ¡Ü 1000) which is the number of datasets that
follow.
</p><p>Each dataset consists of a single line of input containing a vine configuration consisting of a string of
[ and ] characters as described above. The length of the string of [ and ] will be greater than or
equal to zero, and less than or equal to 150.

</p><h3>Output</h3>
<p>For each dataset, you should generate one line of output with the following values: The dataset
number as a decimal integer (start counting at one), a space, and the minimum number of monkeys
required to reach the canopy successfully. Assume that all the hanging vines are reachable from the
jungle floor, and that all monkeys jump on the vines at the same time.

</p><h3>Example</h3>

<pre><b>Input:</b>
3
[]

[[][[]]]

<b>Output:</b>
1 2
2 1
3 8
</pre>