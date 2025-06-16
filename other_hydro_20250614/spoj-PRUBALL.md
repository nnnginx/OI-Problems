<p align="center"><strong></strong><strong>Balls</strong></p>
<p>The classic <em>Two Glass Balls </em>brain-teaser is often posed as: "Given two identical glass spheres, you would like to determine the lowest floor in a 100-story building from which they will break when dropped. Assume the spheres are undamaged when dropped below this point. What is the strategy that will minimize the worst-case scenario for number of drops?" Suppose that we had only one ball. We'd have to drop from each floor from 1 to 100 in sequence, requiring 100 drops in the worst case. Now consider the case where we have two balls. Suppose we drop the first ball from floor <strong><em>n</em></strong>. If it breaks we're in the case where we have one ball remaining and we need to drop from floors 1 to <strong><em>n</em></strong>-1 in sequence, yielding <strong><em>n </em></strong>drops in the worst case (the first ball is dropped once, the second at most <strong><em>n</em></strong>-1 times). However, if it does not break when dropped from floor <strong><em>n</em></strong>, we have reduced the problem to dropping from floors <strong><em>n</em></strong>+1 to 100. In either case we must keep in mind that we've already used one drop. So the minimum number of drops, in the worst case, is the minimum over all <strong><em>n</em></strong>. You will write a program to determine the minimum number of drops required, in the worst case, given <strong><em>B </em></strong>balls and an <strong><em>M</em></strong>-story building.</p>
<p><strong>Input</strong></p>
<p><strong>&nbsp;</strong>The first line of input contains a single integer <strong><em>P</em></strong>, (1 ¡Ü <strong><em>P </em></strong>¡Ü 1000), which is the number of data sets that follow. Each data set consists of a single line containing three (3) decimal integer values: the problem number, followed by a space, followed by the number of balls <strong><em>B</em></strong>, (1 ¡Ü <strong><em>B </em></strong>¡Ü 50), followed by a space and the number of floors in the building <strong><em>M</em></strong>, (1 ¡Ü <strong><em>M </em></strong>¡Ü 1000).</p>
<p>&nbsp;<strong>Output</strong></p>
<p><strong>&nbsp;</strong>For each data set, generate one line of output with the following values: The data set number as a decimal integer, a space, and the minimum number of drops needed for the corresponding values of <strong><em>B </em></strong>and <strong><em>M</em></strong>.</p>
<p><strong>Sample Input</strong></p>
<p>4</p>
<p>1 2 10</p>
<p>2 2 100</p>
<p>3 2 300</p>
<p>4 25 900<strong></strong></p>
<p><strong>Sample Output</strong></p>
<p>1 4</p>
<p>2 14</p>
<p>3 24</p>
<p>4 10<strong></strong></p>