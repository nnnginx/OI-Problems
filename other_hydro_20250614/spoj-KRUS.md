<p>Aladdin has become bored of life at the palace. He has a steady job, his wife Jasmine, kids are on the way and life is becoming monotonous. Prompted by all this, he has decided to have one more adventure before settling down.</p>
<p>He has decided to find the Golden Pear, an extremely valuable legendary artifact that no one has been able to find.</p>
<p>The desert Aladdin is searching is can be modeled as an N¡ÁN grid of cells. Rows and columns are numbered 1 through N top to bottom and left to right. Some of the cells in the desert contain wizards that help Aladdin's quest in an unusual way.</p>
<p>Aladdin starts his quest in the top left corner of the desert on a Monday facing right. His movement involves repeating these steps:</p>
<ul>
<p>1. If the current cell contains a wizard that is awake, then Aladdin turns 90 degrees left or right, depending on what the wizard says.</p>
<p>2. If moving forward would take Aladdin out of desert, he turns 180 degrees.</p>
<p>3. Aladdin moves forward one cell and it takes him exactly one day.</p>
</ul>
<p>For each wizard we know his location and his activity schedule for each day of the week. The schedule is a string of exactly seven letters 'L', 'R' or 'S', each character telling us what the wizard does on one day of the week (starting with Monday). The letter 'L' means that Aladdin will be told to turn left, 'R' that Aladdin will be told to turn right, while 'S' means the wizard sleeps that day.</p>
<p>An old prophecy says that after K changes in direction (in steps 1 and/or 2) Aladdin will find the Pear.</p>
<p>Write a program that calculates how many days the search will last, according to the ancient prophecy.</p>
<h3>Input</h3>
<p>The first line contains two integers N and K (2 ¡Ü N ¡Ü 200, 1 ¡Ü K ¡Ü 1 000 000 000), the size of the desert and the number of direction changes in the prophecy.</p>
<p>The second line contains an integer M (0 ¡Ü M ¡Ü 10 000), the number of wizards.</p>
<p>Each of the following M lines contains two integers R and C (1 ¡Ü R, C ¡Ü N), and a string of seven letters 'L', 'R' or 'S'. The numbers represent the row and column where the wizard is located, while the string is his schedule.</p>
<p>No two wizards will share the same cell, nor will there be a wizard in cell (1, 1).</p>

<h3>Output</h3>
<p>Output the length of the search in days.</p>

<h3>Example</h3>

<pre><b>Input:</b>
5 2
2
1 3 RRSRRRR
1 5 RRRRLRR

<b>Output:</b>
4
</pre>