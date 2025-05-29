<p>Rarity is collecting special crystals for the upcoming Equestria games.  Currently, she is in a gem cave and has found a bunch of crystals.
</p><p>To Rarity's discerning eye, crystals have three properties: a color, a reactivity level, and a fashion value.
Of course, Rarity wants to collect crystals to maximize the total fashion value.

</p><p>Rarity knew she wouldn't have enough room in just one bag for all the crystals, so she brought two.

</p><p>Well, it turns out that space isn't the main issue that Rarity has.  These special crystals are reactive.
In their current environment, they are relatively stable, but once Rarity has put them in her bag and
taken them out of the gem cave, if the reactivity levels are too high, the gems will disintegrate, and thus lose all their fashion value.

</p><p>There are two ways that reactions can happen:
</p><ol>
<li>If there are too many gems of the same color, in the same bag, they'll disintegrate.</li>
<li>If the total reactivity level of the crystals in the same bag is too high, they'll disintegrate.</li>
</ol>

<p>Different colors of gems have different reaction limits.  Also, it is possible that some colors of gems are simply unstable and will always disintegrate when taken outside the cave.

</p><p>Twilight Sparkle had studied these crystals at some point, and discovered a way to stop crystals from reacting.  The material is difficult to create, but she has still given Rarity a separate, special bag which can hold only a single crystal, but that crystal won't react no matter what while it is in the bag.

</p><p>This is the situation Rarity is in, and she needs your help.

</p><h3>Input</h3>
<p>You will be given T, the number of test cases to follow.
</p><p>Each test case begins with a single line containing the values R and C
<br>R is the maximum reactivity level allowed in a regular bag without having the crystals disintegrate.
<br>C is the number of different colors of gems that Rarity currently can see.

</p><p>The next C lines will be of the form L N r_1 v_1 r_2 v_2 ... r_N v_N.
<br>L is the limit for how many crystals of this color can be in the same bag without reacting.
<br>N is the number of crystals of this color that Rarity can see.
<br>The next 2*N numbers are pairs indicating the reactivity level and the fashion value of each of the N gems.

</p><p>Test cases will follow immediately after each other (see sample input)

</p><p>Limits:
<br>1 &lt;= R &lt;= 100
<br>1 &lt;= C &lt;= 10
<br>0 &lt;= L &lt;= 3
<br>1 &lt;= N &lt;= 10

</p><p>For any reactivity level 'r' or fashion value 'v', 1 &lt;= r, v &lt;= 1000

</p><p>Note that Rarity's two regular bags are large enough to hold any number of crystals.

</p><h3>Output</h3>
<p>For each test case, on a separate line, output the maximum fashion value of the crystals that Rarity is able to collect
in her bags.

</p><h3>Example</h3>

<pre><b>Input:</b>
2
10 2
1 2 5 1 5 1
2 2 6 1 6 1
5 3
3 3 1 1 1 1 1 1
3 3 1 1 1 1 1 1
3 3 1 1 1 1 1 1

<b>Output:</b>
3
9
</pre>
<p> Final note: The time limit for each test case is at a minimum, x3 my Java solution.  There are a few files with the input being 1-2MB.<br>
</p>