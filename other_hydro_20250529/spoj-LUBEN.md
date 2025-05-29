<p>Children in school are having fun instead of listening to the teacher. With their iPhone devices the children throw watermelons at each other on the Facebook social site.</p>
<p>The game started when Goran threw one watermelon at each of his friends during the first class that day. During subsequent classes, all children (including Goran) behaved like this:
</p><ul>
<li>If they had been hit by an odd number of watermelons during the previous class, they threw exactly one watermelon at each of their friends;</li>
<li>If they had been hit by an even number of watermelons (including zero), then they hit each of their friends with two watermelons.</li>
</ul>
<p></p>
<p>The children are numbered 1 through N, Goran obviously being number 1. The friend relationships between the children are also known.</p>
<p>Write a program that will calculate the total number of watermelons thrown after H classes.</p>

<h3>Input</h3>
<p>The first line contains two integers N and H (1 ¡Ü N ¡Ü 20, 1 ¡Ü H ¡Ü 1 000 000 000), the number of kids and classes.</p>
<p>Each of the following N lines contains a string of N characters '0' or '1'. The character (A, B) in this matrix is '1' if children A and B are friends.</p>
<p>No child will be their own friend. The input matrix will be symmetric</p>

<h3>Output</h3>
<p>Output the number of watermelons after H classes.</p>

<h3>Example</h3>

<pre><b>Input:</b>
5 3
01000
10110
01000
01001
00010

<b>Output:</b>
26
</pre>