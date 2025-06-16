<h1>Library for Madrid</h1>
<p>Good preparation is essential for winning programming contests. Thus, if you read this document, you're on the right track ;) Knowing your algorithms and the programming language you use is of prime importance. However, you don't have to learn everything by heart; each team is allowed to bring 25 pages of documentation to the contest.</p>
<p>Now the difficult question is: What should you put on those 25 pages? You know that you can fit 10 paragraphs of text on a page, but your stock of useful code snippets and handy texts is much larger than that. To make things more complicated, some topics depend on each other. You cannot include the line-circle intersection formula if you do not also include the code for lines, circles and points.</p>
<p>As a programmer, you decide to let your computer do the hard work for you. Given a set of topics, their space requirements and dependencies, write a program that prints the maximum number of topics that fit into the library.</p>
<h3>Input</h3>
<p>The input consists of several testcases. Each problem description starts with the numbers 1&nbsp;¡Ü&nbsp;<em>M</em>&nbsp;¡Ü&nbsp;100 and 0&nbsp;¡Ü&nbsp;<em>D</em>&nbsp;¡Ü 10, the number of topics and the number of dependencies. The following <em>M</em> lines contain the name of a topic (one word) and the number <em>L<sub>t</sub></em> of paragraphs (1&nbsp;¡Ü&nbsp;<em>L<sub>t</sub></em>&nbsp;¡Ü&nbsp;1000) of the topic, separated by a space.&nbsp; The next <em>D</em> lines each contain two topic names separated by space, indicating that the first topic depends on the second.</p>
<p>The input file ends with a testcase having <em>M</em>=0, which should not be processed.</p>
<h3>Output</h3>
<p>For each test case, print a single line containing the maximum number of topics that you can fit in the library, followed by the number of free paragraphs that remain. If several solutions yield the same number of topics, choose the one that leaves as much empty space as possible.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>5 4<br>Dijkstra 50<br>Intersections 30<br>Lines 70<br>Circles 120<br>Points 40<br>Intersections Lines<br>Intersections Circles<br>Lines Points<br>Circles Points<br><br>0 0<br><br><strong>Output:</strong><br>3 90<br></pre>
<h3>Notes</h3>
<p>The sample output corresponds to choosing Dijkstra's algorithm, lines and<br>points.</p>