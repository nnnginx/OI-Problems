<p>Surprisingly, the king of the Quadruple Island Kingdom suddenly declares war on its neighbor country, the Utopia Land. After that, the King dispatches a large number of tanks for first attack. You, as the Defense Minister of Utopia Land, are certainly under mass of pressure. In order to defense the enemy, you decide to use the new secret weapon: laser cannon. This kind of weapon is so powerful that can easily destroy any thing at a line in a moment, or course, including tanks.
</p><p>However, Because of some designing flaw, you can use such weapon just once during the war. The only hope is that you can choose a good moment and right way to use it so that as many tanks as possible can be destroyed.
</p><p>A tank can be described as a point whose coordinate is (X<sub>i</sub>, Y<sub>i</sub>) on a 2D-plain with speed vector (VX<sub>i</sub>, VY<sub>i</sub>) per second. Starting at time 0, you can use your laser cannon at any position and in any direction at any INTEGER number of seconds after time 0. It is possible that some tanks will meet at the same point while moving, and they will not influence each other anyway.

</p><h3>Input</h3>

<p>Multiple test cases. The number of test cases is no more than 10. For each test cases, The first line contains a single integer <b>N</b> (1 &lt;= <b>N</b> &lt;= 100) indicating the number of tanks. Then <b>N</b> lines are following that describing the tanks respectively. Each of them consists of four nonzero integer X<sub>i</sub>, Y<sub>i</sub>, VX<sub>i</sub>, VY<sub>i</sub> separated by single spaces where |X<sub>i</sub>|,|Y<sub>i</sub>| &lt;= 100,000,000 and |VX<sub>i</sub>|,|VY<sub>i</sub>| &lt;= 100 denoting the initial position of a tank and the speed vector. Input ends with <b>N</b> = 0.

</p><h3>Output</h3>

<p>For each test case, output one line with a single integer indicating the largest number of tanks which can be destroyed by the laser cannon.
</p><p>Note: Be careful when handling floating point errors.
</p><h3>Example</h3>
<pre><b>Input:</b>
4
10 10 -1 -1
3 1 4 6
2 8 5 -1
1 3 1 4
0

<b>Output:</b>
3
</pre>