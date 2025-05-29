<p>It's Christmas morning, and you've got what you wanted: a box of Lego™! (Okay, maybe not, but better than nothing)<br> <br> Lego is pretty fun to tinker with, and you've decided to build some sort of shape.<br> (For the sake of this problem, let's say your shape is basically 2-dimensional - it'll be a slab)<br> <br> But once you pick it up, you discover that you didn't plan it properly, and your wonderful shape just falls apart.<br> Now, you're planning to build something big, and so you're going to use the computer to help you.<br> Write a program, that given the layout of a Lego design, outputs the number of pieces it would break into if picked up.<br> (Assume that the bricks bind together perfectly)<br> <br> The Legos will be built on a x-y coordinate plane, with (0,0) being the bottom left corner.<br> The blocks are flat on your carpet, so a block will never 'fall down'.<br> (If you haven't seen a Lego brick before: A Lego brick has grooves on its top that match with notches on the bottom.<br> If a groove and a notch bind, the bricks will stay together. See the diagram.<br> A brick will bind with another brick securely even if just a single notch touches another groove.</p>
<h3>Input:</h3>
<p>The first line contains <em>N</em> (the number of Lego pieces), 1 ≤ <em>N</em> ≤ 100000.<br> <em>N</em> lines follow, each with 4 integers <em>x</em><sub>1</sub>, <em>y</em><sub>1</sub>, <em>x</em><sub>2</sub>, <em>y</em><sub>2</sub> (0 ≤ <em>x</em><sub>1</sub> &lt; <em>x</em><sub>2</sub> ≤ 2×10<sup>9</sup>, 0 ≤ <em>y</em><sub>1</sub> &lt; <em>y</em><sub>2</sub> ≤ 2×10<sup>9</sup>)<br> <br> This means that there is a brick with bottom left corner (<em>x</em><sub>1</sub>,<em>y</em><sub>1</sub>) and top right corner (<em>x</em><sub>2</sub>,<em>y</em><sub>2</sub>). <em>x</em> denotes the horizontal coordinate and <em>y</em> the vertical coordinate. Two bricks will bind if one's bottom <em>y</em>-coordinate coincides with the other's top <em>y</em>-coordinate and the intersection of the two intervals (the bottom of one and the top of the other) has nonzero length.<br> No bricks will overlap.</p>
<h3>Output:</h3>
<p>A single line containing the number of separate pieces that these blocks form.</p>
<h3>Sample Input:</h3>
<pre>4
0 0 2 2
1 2 3 4
2 0 4 2
4 0 6 2</pre>
<h3>Sample Output:</h3>
<pre>2</pre>
<h3>Explanation</h3>
<p>Blocks #1,2,3 are joined securely.<br> However, #4 is just hanging around.<br> <br> <img src="./23160/file/GRz64bM0.png" alt=""></p>