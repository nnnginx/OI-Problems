<p>Secret Committee members, Little Petar and Little Tux, enjoy playing the board game "Kule" during the breaks between preparing contests and exam revision. The rules of the game assume that the players initially have at their disposal a set of cubes, stacked together to form a tower.</p>
<p>A single turn has Petar splitting the tower into <strong>two or more smaller towers</strong>, and then ordering these smaller towers in an array. Tux then has to <strong>choose</strong> one of the smaller towers. This tower will be used for all future turns, while the remainder is <em>discarded</em>. If Tux chooses the kth tower,<strong> Petar is obliged to pay k<sup>2</sup>&nbsp;dinars to him immediately </strong>(e.g. if Tux chose the 3rd tower in the array, Petar has to give him 9 dinars). The game concludes <em>when only a single cube remains</em>.</p>
<p>As it is well-known that Secret Committee members don't have time for anything (including playing games), Petar and Tux decided to, instead of actually playing the game, trust each other that they would have played <strong>optimally</strong>, and that Petar should immediately give Tux the amount of dinars that he would have won under that condition. They have asked for your help in determining this amount.</p>
<h3>Input</h3>
<p>The first and only line of the standard input contains a single integer N, the number of cubes in the initial tower.</p>
<h3>Output</h3>
<p>Write to the first and only line of the standard output a single integer M, representing the amount of dinars that Petar should give to Tux.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
7

<strong>Output:</strong>
8</pre>
<p>&nbsp;</p>
<h3>Explanation</h3>
<p>In one of the possible pair of optimal strategies for Petar and Tux, Petar first splits the tower into two towers of heights 5 and 2 (in that order). Tux chooses the second tower and he immediately gets 4 dinars, after which Petar is forced to split the tower into two towers of heights 1 each. Tux once again chooses the second tower, gaining a total of 8 dinars.</p>
<h3>Constraints</h3>
<ul>
<li>2 &lt;= N &lt;= 10<sup>100</sup></li>
</ul>
<p>&nbsp;</p>