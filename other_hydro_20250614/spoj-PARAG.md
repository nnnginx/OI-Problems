<p>Ever heard of paragliding? It's a recreational sport in which one jumps off an elevated position, and then soars through the sky equipped with a 'paraglider' (a parachute of sorts). Although air currents might help you out, gravity will relentlessly pull you towards the ground eventually.</p>
<p>As all good sports, paragliding has a group of enthusiasts in Slovakistan, who call themselves 'Klub Slovakistanských Paraglidistov' (KSP). And as all real enthusiast groups, KSP organizes club activities - group tours to the most prestigious paragliding centers, where all members of the club can paraglide to their hearts' content in the most luxurious mountain ranges. Of course, every upcoming tour must be more awesome than the last, and so the selection of the right destination is key. It will be extra important this year, as the Slovakistan paragliding superstar Syseľ agreed to come along. With his dedication and love for the sport, he is recognized on the worldwide paragliding scene.</p>
<p>In his bestseller autobiography the members of KSP have read that Syseľ enjoys long flights the most - such that the difference of the heights of the mountain he jumps from and lands on is greater than <strong>m</strong>. In the context of an exclusive interview he mentioned that what he most dislikes about paragliding is the need to climb up onto a mountain after every jump; hence, he usually likes to jump from a tall mountain, land on a smaller one, and immediately jump again from this smaller mountain, and so on. If he does this <strong>s-1</strong> times, he is satisfied. Lastly from an intercepted phone call KSP members concluded that Syseľ likes to paraglide after lunch, but only in the eastwards direction, as when he paraglides to the west the sun shines into his eyes.</p>
<p>KSP does not want to disappoint Syseľ, and hence they are looking for such a mountain range which has the most possible trips which satisfy Syseľ. Help them!</p>
<h3>Task</h3>
<p>Every mountain range consisting of <strong>n</strong> mountains can be described as an array of <strong>n</strong> numbers, representing the heights of these mountains from west to east.</p>
<p>A trip is an arbitrary sequence of several, not necessarily neighbouring mountains, which satisfies Syseľ if and only if it contains exactly <strong>s</strong> mountains, and between each two consecutive mountains in this sequence the difference in elevation is greater than <strong>m</strong> - that is if a mountain's height is <strong>x</strong>, and the nearest mountain to the east on the trip has a height of <strong>y</strong>, then <strong>x-y&gt;m</strong>.</p>
<p>For a given mountain range consisting of <strong>n</strong> mountains and the values of <strong>m</strong> and <strong>s</strong>, find the number of trips which exist in this mountain range that satisfy Syseľ.</p>
<h3>Input</h3>
<p>There are multiple test cases - their number<strong>&nbsp;1 ≤ T ≤ 70</strong>&nbsp;will be on the first line.</p>
<p>The first line of each test case contains the integers <strong>1 ≤&nbsp;</strong><strong>n ≤ 10<sup>5</sup></strong>, <strong>0 ≤&nbsp;</strong><strong>m ≤ 10<sup>18</sup></strong>&nbsp;and <strong>2 ≤&nbsp;</strong><strong>s ≤ 20</strong>: the number of mountains in the mountain range, the required difference in elevation, and the number of mountains in a trip which satisfies Syseľ.</p>
<p>The second line of each test case contains&nbsp;<strong>n</strong> numbers - the heights of the mountains in the mountain range, from west to east. The heights of mountains are positive integers not greater than <strong>10</strong><sup><strong>18</strong></sup>.</p>
<p>The sum of <strong>n</strong>&nbsp;within one input file does not exceed <strong>400,000</strong>.</p>
<h3>Output</h3>
<p>For each test case output the string "Case <strong>x</strong>: <strong>y</strong>", where <strong>x</strong> is the number of the test case, starting from 1, and <strong>y</strong> is the number of trips in the mountain range that satisfy Syseľ, modulo <strong>10<sup>9</sup>+7</strong>. We consider two trips distinct if there exists at least one mountain which belongs to one trip but not the other.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
4 0 2
5 4 3 1
4 1 2
5 4 3 1
8 3 3
11 15 15 10 10 7 1 1
<strong>Output:</strong>
Case 1: 6
Case 2: 4
Case 3: 14</pre>
<p>In the first case, any pair of mountains is a trip which satisfies Syseľ. In the second case, the pairs of mountains with heights (5,4) and (4,3) no longer have a great enough elevation difference.</p>