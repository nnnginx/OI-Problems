<p> Ada the Ladybug owns a circular land. She wants to enclose it with fence.
Anyway since nobody sells round planks, she has decided to fence it to shape of
regular <b>k-gon</b>. Problem is, that there is only limited number or places
(on circle) where pilars can be built. Ada has asked you, to find out the
number of different regular <b>k-gon</b> shaped fences which can be built on her
land (two <b>k-gon</b>'s are considered different if they share NO common pillar).

</p><h3>Input</h3>
The first line will contain <b>T</b>, the number of test-cases.
<p>Then <b>T</b> test-cases follow, each beginning with two integers <b> 3
    ¡Ü K ¡Ü N ¡Ü 10<sup>5</sup></b>, <b>3 ¡Ü K ¡Ü 100</b>, the number
of places where pillar can be built and number of edges of regular <b>k-gon</b>

</p><p>Afterward a line with <b>N</b> integers <b>1 ¡Ü D<sub>i</sub> ¡Ü 100
</b>follow, meaning the length of arc between two consecutive points where
pillar can be built. The sum of all lengths will be divisible by <b>K</b>.
</p><p>Sum of <b> N </b> over all test-cases won't exceed <b>2*10<sup>6</sup></b>

</p><h3>Output</h3>
For each test-case print the number of different regular <b>k-gon</b> shaped fences which can be
built.

<h3>Example Input</h3>
<pre>3
5 3
1 2 3 2 1
15 4
1 2 2 2 1 2 2 1 1 2 1 2 1 2 2
10 5
1 1 1 1 1 1 1 1 1 1
</pre>
<h3>Example Output</h3>
<pre>1
1
2
</pre>