<p>Kate is preparing a party. She have bought a very strange garland for it. The garland is a closed chain of bulb. Each bulb can be in one of the following states: N - don't glow, R - glow red, G - glow green, B - glow blue. Each second the state of each bulb changes according to the following table:</p>
&nbsp;<table align="center" border="1" cellpadding="3" cellspacing="0">
<tbody><tr><td></td><td>N</td><td>R</td><td>G</td><td>B
</td></tr><tr><td>N</td><td>N</td><td>R</td><td>G</td><td>B</td></tr><tr>
</tr><tr><td>R</td><td>R</td><td>N</td><td>B</td><td>G</td></tr><tr>
</tr><tr><td>G</td><td>G</td><td>B</td><td>N</td><td>R</td></tr>
<tr><td>B</td><td>B</td><td>G</td><td>R</td><td>N</td></tr>
</tbody></table>
<p>where row is chosen by the current state of the bulb and column is chosen by the state of the bulb on the right. The value at the intersection of the chosen row and column gives the new state of the bulb. For example, if the  bulb glows red (R) and the bulb on its right glows green (G) then in the next second the bulb will glow blue (B). And if the bulb and its right neighbour both glow blue then the bulb won't glow at all in the next second. Also all the bulbs change their states simultaneously. Such behaviour should (theoretically) lead to constant twinkling of the garland. Unfortunately it turns out that sometimes eventually the garland goes into such a state that all bulb don't glow. So the garland stops twinkling. Kate is rather worried that this can spoil the party. She is going to set the initial states of each bulb as she like. Help her determine for how long the garland will twinkle starting from this initial state.</p>

<h3>Input</h3>
<p>The input file consists of a single string containing characters 'N', 'R', 'G' and 'B', which describes the initial state of the garland. Each character defines the initial state of some bulb. The bulbs are listed from left to right. There is the first bulb on the right of the last one. The length of the string will be no more than 1234567 characters.

</p><h3>Output</h3>
<p>Print the number of seconds during which the garland will twinkle. If the garland won't stop twinkling (at least until the power is turned off) print "Party!" (quotes for clarity).

</p><h3>Example</h3>

<pre><b>Input:</b>
RGBG

<b>Output:</b>
4

</pre>

<h3>Explanation</h3>
<p>The garland will change the state in such a way:
</p><pre>RGBG
BRRB
GNGN
GGGG
NNNN
</pre>