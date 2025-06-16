<p>A good war commander must take quick decisions, and at the same time be a good strategist. One of the functions of the commander is to delegate soldiers to several strategic points, such that the enemy can be caught surprised and be defeated. There are several strategic points at the battle field, as well as several routes that connect these points.</p>
<p>Your field is, however, being bombarded, and these routes are not so safe as they were. Once a bomb falls at one route, such terrain becomes irregular and your crossing becomes impossible. To deal with such problem, the commander ordered a new task to some soldiers: find new routes.</p>
<p>The commander asked your help to calculate the shortest path between the base of operation and the strategic points. You will be informed about the initial state of the battle field, with <strong>N</strong> strategic points (being the point 1 the base of operation) and <strong>M</strong> routes. As the bombs falls over some routes, and other routes are found by the soldiers, you must update your map such that your commander can make good use of such information.</p>
<p>Good luck, the country depends on you.</p>
<h3>Input</h3>
<p>The input contains several test cases. Each test case begins with two integers, <strong>N</strong> and <strong>M</strong> (2 �� <strong>N</strong> �� 1000 and 1 �� <strong>M</strong> �� 10000), representing, respectively, the number of strategic points and the number of routes that connects two strategic points. After that, there will be <strong>M</strong> lines, each one with three integers <strong>U</strong>, <strong>V</strong> and <strong>W</strong> (1 �� <strong>U</strong>, <strong>V</strong> �� <strong>N</strong> and 1 �� <strong>W</strong> �� 100) each, representing that there is a route that connects the point <strong>U</strong> to the point <strong>V</strong>, in unique direction, with distance <strong>W</strong>.</p>
<p>There will be, then, an integer <strong>Q</strong> (1 �� <strong>Q</strong> �� 1000), that represents the number of consults or updates that will be done over the routes. At the next <strong>Q</strong> lines there will be a letter and a determined number of integers.</p>
<p>If the letter is a <strong>R</strong>, there will be two integers <strong>U</strong> and <strong>V</strong> (1 �� <strong>U</strong>, <strong>V</strong> �� <strong>N</strong>), indicating that the route that used to connect the point <strong>U</strong> to the point <strong>V</strong> was bombed.</p>
<p>In the case that the letter is a <strong>I</strong>, there will be three integers <strong>U</strong>, <strong>V</strong> and <strong>W</strong> (1 �� <strong>U</strong>, <strong>V</strong> �� <strong>N</strong> and 1 �� <strong>W</strong> �� 100), indicating that a new route was found, which connects the point <strong>U</strong> to the point <strong>V</strong>, with distance <strong>W</strong>.</p>
<p>And in the case that the letter is a <strong>P</strong>, there will be one integer <strong>V</strong> (1 �� <strong>V</strong> �� <strong>N</strong>), and you must inform to the commander what is the shortest distance between the base of operation and the strategic point <strong>V</strong>.</p>
<p>The input ends when <strong>N</strong> = <strong>M</strong> = 0.</p>
<h3>Output</h3>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">A good war commander must take quick decisions, and at the same time be a good strategist. One of the functions of the commander is to delegate soldiers to several strategic points, such that the enemy can be caught surprised and be defeated. There are several strategic points at the battle field, as well as several routes that connect these points.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="white-space: pre;"> </span>Your field is, however, being bombarded, and these routes are not so safe as they were. Once a bomb falls at one route, such terrain becomes irregular and your crossing becomes impossible. To deal with such problem, the commander ordered a new task to some soldiers: find new routes.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="white-space: pre;"> </span>The commander asked your help to calculate the shortest path between the base of operation and the strategic points. You will be informed about the initial state of the battle field, with N strategic points (being the point 1 the base of operation) and M routes. As the bombs falls over some routes, and other routes are found by the soldiers, you must update your math such that your commander can make good use of such informations.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="white-space: pre;"> </span>Good luck, the country depends on you.</div>
<p>For each test case there will be a not defined number of output lines. When the commander order to know the shortest distance between the base of operation and a strategic point (letter <strong>P</strong>), such distance must be print in an unique line. If it is not possible to reach such strategic point, the number -1 must be printed. There must have a blank line after each test case.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre>3 3
1 2 2
2 3 3
1 3 4
5
P 3
R 2 3
P 3
I 2 3 1
P 3</pre>
<pre><strong>Output:</strong></pre>
<pre>4
4
3</pre>