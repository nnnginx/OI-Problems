<p>There are some chickens and rabbits in the cage. They have fifteen heads and forty feet in all. How many chickens and rabbits are there respectively?</p>

<p>It is a classical math problem which can date back to the Northern and Southern Dynasties (420-589). Here is an interesting algorithm to solve the problem: Assume that the chickens and rabbits are well trained. You whistle, and all of them lift a leg, then there are <i>40-15=25</i> feet on the floor. You whistle again, and there are <i>25-15=10</i> legs remain standing. After two whistles, all the chickens sit on the floor, and all the rabbits stand on two legs. So there are <i>10/2=5</i> rabbits and <i>15-5=10</i> chickens.</p>

<p>John has a farm with lots of animals in it. He is now facing the similar problem. There are exactly <b>N</b> kinds of animals and he wants to know their quantities. He only knows that different kinds of animals have different number of legs (at least one), but he has no idea how many legs they each have. He trains the animals and tries to figure it out using the algorithm stated above. First he makes all the animals stand up with all their legs and counts their legs. Then, for each time he whistles, all the animals lift one leg(if it has at least one leg standing on the ground), and then he counts the feet again. After <b>K</b> times, he thinks that it is enough to determine the quantity of each kind of animal, but does it really work? So, it is your job to help him to solve the problem.</p>

<h3>Input</h3>
<p>The first line contains an integer <b>T</b> (1 �� <b>T</b> �� 100), indicating the number of test cases.</p>

<p>Each test case contains two lines. The first line contains two integers <b>N</b> (1 �� <b>N</b> �� 1000) and <b>K</b> (1 �� <b>K</b> �� 1000), representing the number of different kinds of animals and the time he whistles. </p>

<p>The second line contains <b>K</b>+1 integers <b>A</b><sub>0</sub> , <b>A</b><sub>1</sub>... <b>A</b><sub><b>K</b></sub> (0 �� <b>A</b><sub>i</sub> �� 10<sup>4</sup>) where <b>A</b><sub>i</sub> represents the number of legs after his <i>i</i>-th whistle.</p>

<h3>Output</h3>
<p>For each test case in the input, print several lines.</p>

<p>The first line contains <tt>"Case #X:"</tt>, where <b>X</b> is the test case number (starting with 1). The next line contains <tt>"No Solution"</tt>, <tt>"Unique Solution"</tt> or <tt>"Multiple Solutions"</tt> according to the result.</p>

<p>If the result is uniquely determined, you should print <b>N</b> extra lines each contains two integer <b>L</b><sub>i</sub>, <b>N</b><sub>i</sub>, where <b>L</b><sub>i</sub> represents how many legs does the <i>i</i>-th kind of animal have and <b>N</b><sub>i</sub> represents the number of <i>i</i>-th kind of animal. The animals should be sorted by the number of their legs in ascending order.</p>

<h3>Example</h3>

<pre><b>Input:</b>
3
2 3
14 9 6 3
2 2
8 5 3
3 2
20 13 8

<b>Output:</b>
Case #1:
Unique Solution
1 2
4 3
Case #2:
No Solution
Case #3:
Multiple Solutions
</pre>