<p>Nowadays, people have many ways to save money on accommodation when they are on vacation. One of these ways is exchanging houses with other people. </p>

<p>Here is a group of <b>N</b> people who want to travel around the world. They live in different cities, so they can travel to some other people's city and use someone's house temporary. Now they want to make a plan that choose a destination for each person. There are two rules should be satisfied:</p>

<ol>
<li>All the people should go to one of the other people's city.</li>
<li>Two of them never go to the same city, because they are not willing to share a house.</li>
</ol>

<p>They want to maximize the sum of all people's travel distance. The travel distance of a person is the distance between the city he lives in and the city he travels to. These <b>N</b> cities have <b>N</b>-1 highways connecting them. The travelers always choose the shortest path when traveling.</p>

<p>Given the highways' information, it is your job to find the best plan, that maximum the total travel distance of all people.</p>

<h3>Input</h3>
<p>The first line of input contains one integer <b>T</b> (1 ¡Ü <b>T</b> ¡Ü 10), indicating the number of test cases.</p>

<p>Each test case contains several lines.
The first line contains an integer <b>N</b> (2 ¡Ü <b>N</b> ¡Ü 10<sup>5</sup>), representing the number of cities.
Then the following <b>N</b>-1 lines each contains three integers <b>X</b>, <b>Y</b>, <b>Z</b> (1 ¡Ü <b>X</b>, <b>Y</b> ¡Ü <b>N</b>, 1 ¡Ü <b>Z</b> ¡Ü 10<sup>6</sup>), means that there is a highway between city <b>X</b> and city <b>Y</b>, and length of that highway.</p>

<p>You can assume all the cities are connected and the highways are bi-directional.</p>

<h3>Output</h3>
<p>For each test case in the input, print one line: <tt>"Case #X: Y"</tt>, where <b>X</b> is the test case number (starting with 1) and <b>Y</b> represents the largest total travel distance of all people.

</p><h3>Example</h3>

<pre><b>Input:</b>
2
4
1 2 3
2 3 2
4 3 2
6
1 2 3
2 3 4
2 4 1
4 5 8
5 6 5

<b>Output:</b>
Case #1: 18
Case #2: 62
</pre>