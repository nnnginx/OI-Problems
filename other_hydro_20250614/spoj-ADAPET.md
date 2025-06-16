<p>Ada the Ladybug just got herself a new pet. She was thinking about a name for it. She thought-up a beautiful name for it already but now she doesn't think this name is "enough". She wants to find a new name, which will contain the original name at least <strong>K</strong> times as substring (to emphasize its importance). As ada doesn't want the pet's name to be too long, she wants to find the shortest one - can you find the length of it?</p>
<h3>Input</h3>
<p>The first line of input will contain <strong>T</strong>, the number of test-cases.</p>
<p>Each of the next <strong>T</strong> lines will contain a non-empty string <strong>s</strong>, consisting of lowercase-english letters and a number <strong>1 ¡Ü K ¡Ü 10<sup>6</sup></strong> (the number of times the given name shall be in the new name).</p>
<p>The sum of lengths of strings over all test-cases will not exceed <strong>5*10<sup>5</sup></strong>.</p>
<h3>Output</h3>
<p>For each test-case print the minimum length of new name.</p>
<h3>Example Input</h3>
<pre>8
ada 3
abc 2
r 7
rr 5
gorego 3
abbababbbbababababba 2
abcabcabca 3
lopadotemachoselachogaleokranioleipsanodrimhypotrimmatosilphioparaomelitokatakechymenokichlepikossyphophattoperisteralektryonoptekephalliokigklopeleiolagoiosiraiobaphetraganopterygon 1
</pre>
<h3>Example Output</h3>
<pre>7
6
7
6
14
36
16
182
</pre>