<p>Mariusz and Pawel are playing a Prismata game. After many turns the situation is as follows. Pawel has:</p>
<ul>
<li> one Gauss Fabricator, with <em>f<sub>h</sub></em> health, which will produce one Gauss Cannon per turn for the next <em>f<sub>l</sub></em> turns </li>
<li> <em>g</em> Gauss Cannons, each Gauss Cannon has <em>g<sub>h</sub></em> health </li>
</ul>
<p>Mariusz has <em>t</em> Tarsiers. Each Tarsier has one health.<br> The Gauss Cannon and the Tarsier are the units with one attack. This means that the unit inflicts one damage per turn on a one of the opponent's units. A unit that has lost all its health is immediately destroyed. A unit which has only lost part of its health remains fully operational.<br> A single turn in Prismata goes like below:</p>
<ul>
<li> Mariusz attacks. Mariusz decides how many Tarsiers attack the Gauss Fabricator and how many attack the Gauss Cannons. The same Gauss Cannon can be attacked by more than one Tarsier. </li>
<li> Pawel attacks. If Pawel has <em>n</em> Gauss Cannons, then Pawel destroys <em>n</em> Mariusz's Tarsiers (Pawel does not make any decisions). </li>
<li> If the Gauss Fabricator has not yet been destroyed, then it produces one Gauss Cannon with <em>g<sub>h</sub></em> health. Independently of the remaining health, the Gauss Fabricator is destroyed after producing <em>f<sub>l</sub></em> Gauss Cannons. Pawel can start attacking with the new Gauss Cannon in the next turn. </li>
</ul>
<p>The player who destroys all the opponent's units wins.<br> Your task is to help Mariusz to find out whether he can win the game and calculate the minimum number of turns needed for the victory.</p>
<h3>Input</h3>
<p>The first line contains the number of tests <em>T(1 ¡Ü T ¡Ü 10)</em>. Each of the&nbsp;<em>T</em> next lines contains one test. A single test consists of:</p>
<ul>
<li> <em>f<sub>h</sub> (1 ¡Ü f<sub>h</sub> ¡Ü 1000000)</em> - the health of the Gauss Fabricator </li>
<li> <em>f<sub>l</sub> (1 ¡Ü f<sub>l</sub> ¡Ü 1000000)</em> - the maximum number of produced Gauss Cannons by the Gauss Fabricator </li>
<li> <em>g<sub>h</sub> (1 ¡Ü g<sub>h</sub> ¡Ü 1000)</em> - the health of a single Gauss Cannon </li>
<li> <em>g (0 ¡Ü g ¡Ü 1000000)</em> - the initial number of Gauss Cannons </li>
<li> <em>t (1 ¡Ü t ¡Ü1000000)</em> - the initial number of Tarsiers </li>
</ul>
<h3>Output</h3>
<p>For each test your program should output:</p>
<ul>
<li> "PAWEL" if Mariusz is unable to win the game </li>
<li> "MARIUSZ t" if Mariusz can win the game and <em>t</em> is the minimum number of turns needed for the victory </li>
</ul>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
5 100 2 5 7
100 3 10 0 8
100 1 60 0 10

<strong>Output:</strong>
MARIUSZ 4
MARIUSZ 6
PAWEL
</pre>
<h3>Explanation of the sample tests</h3>
<p><strong>Test 1</strong>: If left alone, the Gauss Fabricator will produce too many cannons. Therefore Mariusz has to destroy it. One of the possible way for Mariusz to win is:</p>
<p>Turn #1: Mariusz: 7 Tarsiers, Pawel: 5 Gauss Cannons (each with 2 health), the Gauss Fabricator has 5 health</p>
<ul>
<li>Mariusz destroys 3 cannons and inflicts one damage on one of the remaining cannons. </li>
<li>Pawel has 2 cannons. He destroys 2 Tarsiers. </li>
<li>The Gauss Fabricator produces one cannon. </li>
</ul>
<p>Turn #2: Mariusz: 5 Tarsiers, Pawel: 3 Gauss Cannons (2 Gauss Cannons with 2 health, one Gauss Cannon with 1 health), the Gauss Fabricator has 5 health</p>
<ul>
<li>Mariusz destroys all 3 cannons. </li>
<li>Pawel hasn't got any cannons, all Tarsiers remain. </li>
<li>The Gauss Fabricator produces one cannon. </li>
</ul>
<p>Turn #3: Mariusz: 5 Tarsiers, Pawel: 1 Gauss Cannon with 2 health, the Gauss Fabricator has 5 health</p>
<ul>
<li>Mariusz destroys one cannon and inflicts 3 damage on the Gauss Fabricator. </li>
<li>Pawel hasn't got any cannons, all Tarsiers remain. </li>
<li>The Gauss Fabricator produces one cannon. </li>
</ul>
<p>Turn #4: Mariusz: 5 Tarsiers, Pawel: 1 Gauss Cannon with 2 health, the Gauss Fabricator has 2 health</p>
<ul>
<li>Mariusz destroys one cannon and the Gauss Fabricator. </li>
</ul>
<p><strong>Test 2</strong>: In this test the Gauss Fabricator has a lot of health but will produce only few cannons. Mariusz should attack only the cannons and wait for the Gauss Fabricator to be destroyed after 3 turns.</p>
<p><strong>Test 3</strong>: Even though the Gauss Fabricator will produce only one cannon, the health of this cannon is too high for Mariusz to win.</p>