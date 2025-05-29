<p>Snow White and the N dwarfs live in the forest. While the dwarfs mine away Snow White hangs&nbsp;around social networks.</p>
<p>Each morning the dwarfs form a long line and go whistling away to the mine. Snow White runs around&nbsp;them and snaps pictures to upload onto her favorite social network.</p>
<p>When dwarfs enter the mine, Snow White goes back to their house and goes through the pictures,&nbsp;selecting pretty ones. Each dwarf has a colored cap, and there are C different colors. A picture is pretty&nbsp;if more than half caps on it are of the same color. In other words, if there are K dwarfs on the picture,&nbsp;it is pretty if strictly more than K / 2 dwarfs have same colored caps.</p>
<p>Write a program that will check for a set of M pictures if they are pretty, and what color is dominating&nbsp;if they are.</p>
<h3><strong>Input</strong></h3>
<p>First line contains two integers N and C (3 ¡Ü N ¡Ü 300000, 1 ¡Ü C ¡Ü 100000) number of dwarfs and&nbsp;number of colors.</p>
<p>Second line contains N integers between 1 and C (inclusive), colors of dwarves hats, ordered the way&nbsp;they formed the line that morning.</p>
<p>Third line contains M (1 ¡Ü M ¡Ü 100000), number of pictures.</p>
<p>Next M lines contain two integers A and B (1 ¡Ü A ¡Ü B ¡Ü N). Each line describes one picture. On it&nbsp;there are all dwarves starting from A-th all the way to the B-th.</p>
<h3>Output</h3>
<p>Output M lines. For each picture output ¡°no¡± if Snow White doesn't think the picture is pretty, and&nbsp;¡°yes X¡±, where X is the color dominating on the picture, if she does.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
10 3
1 2 1 2 1 2 3 2 3 3
8
1 2
1 3
1 4
1 5
2 5
2 6
6 9
7 10

<strong>Output:</strong>
no
yes 1
no
yes 1
no
yes 2
no
yes 3<span style="white-space: normal;">
</span></pre>