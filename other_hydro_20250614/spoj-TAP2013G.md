<p><strong><em>[The original version of this problem (in Spanish) can be found at <a title="http://www.dc.uba.ar/events/icpc/download/problems/tap2013-problems.pdf" href="http://www.dc.uba.ar/events/icpc/download/problems/tap2013-problems.pdf">http://www.dc.uba.ar/events/icpc/download/problems/tap2013-problems.pdf</a>]</em></strong></p>
<p>War, an event worthy only of appearance in literature, movies or perhaps programming contests, has reached the Nlogonian empire, which is facing the neighboring empire of Quadradonia.</p>
<p>War protocols agreed upon by both parties indicate that the war will be waged in successive battles, in each of which a different soldier from each empire will face one another, so that each soldier will take part in exactly one battle. The empire that wins more battles will then win the war.</p>
<p>Each empire has an army formed by <strong>S</strong> soldiers, and each soldier has a certain combat skill. In each battle between two soldiers, the one with greatest combat skill wins the battle. If both soldiers have the same combat skills, the battle is declared a draw and technically no side claims victory. The spies of Nlogonia have intercepted secret information concerning the combat skill of each soldier of Quadradonia's army, so Nlogonia's queen requires your assistance in order to calculate the maximum number of battles that can be won during the war if her soldiers are sent in the appropriate order.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line contains an integer number <strong>S</strong> representing the number of soldiers in each army (<strong>1 ¡Ü&nbsp;S&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;10<sup>5</sup></strong>). The second line contains <strong>S</strong> integer numbers <strong>Q<sub>i</sub></strong> representing the combat skills of the different soldiers of Quadradonia's army, in the order in which the battles shall take place (<strong>1&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;Q<sub>i</sub>&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;10<sup>9</sup></strong> for <strong>i = 1, ..., S</strong>). The third line contains <strong>S</strong> integer numbers <strong>N<sub>i</sub></strong> representing the combat skills of the different soldiers in Nlogonia's army, in an arbitrary order (<strong>1&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;N<sub>i</sub>&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;10<sup>9</sup></strong>&nbsp;for <strong>i = 1, ..., S</strong>).</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>Print a line containing a single integer number representing the maximum number of battles that Nlogonia can win during the war.</p>
<p>&nbsp;</p>
<h3>Example 1</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">3
2 1 1000000000
1 1 2</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">1</span></pre>
<h3>Example 2</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">4
6 3 1 4
2 7 4 3</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">3</span><span style="white-space: normal;">
</span></pre>