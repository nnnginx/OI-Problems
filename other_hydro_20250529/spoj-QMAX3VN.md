<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/QMAX3VN/en/">English</a></td>
<td width="50%"><a href="/problems/QMAX3VN/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>Following the journey to explore the real power of special data stuctures, two adventurers <strong><em>pirate</em></strong> and <strong><em>duyhung123abc</em></strong> continued to find new challenges with new more and more complicated problems. But what they earned was unremarkable. Being tired and stucked, they decided to review the problems they had solved to see what they had had so far. Suddenly, a mysterious light came to their mind: <em>"why not combine some of them into one !"</em>. And here, <strong>QMAX3VN</strong> was born, as natural as the way fire had come to humankind.</p>
<p>It is said that in a morning at a military camp. All soldiers were gathering in a line to prepare for morning excercises. But the problem was they did not get up simultaneously. The line was initially empty. After sometime, a soldier got up and ran hurrily to join the line. Also, each of them liked to stand near their friends so they would elbow themselves to some position of the current line. What a messy and unacceptable scene for a military camp! The soldiers knew what they had done and were ready to be punished. The strict commander decided to give them a lesson. Everytime he gave an <strong>order(x,y)</strong>, all soldiers in the line had to say loudly the height of <strong>the highest man</strong> among those were standing from position x to position y. Orders were made <strong>continuously</strong> since the first soldier entered the line. Punishment was waiting for whom would carried out the order incorrectly. The yard was full of worry from young soldiers. They really needed help !</p>
<h3>Input</h3>
<p>The input contains several lines:</p>
<ul>
<li> Line 1 : An integer n (1 �� n �� 100000): The number of events occuring in that morning.</li>
<li> Line 2 to line n+1: Each line is one of the following two events:    
<ul>
<li><strong>A x y</strong> : A soldier with height x had just entered the line and elbowed himself into the position between position y-1 and position y of the line (-10<sup>9</sup> �� x �� 10<sup>9</sup>; 1 �� y �� k+1 , k denotes the number of soldiers in the line right before this soldier came).</li>
<li><strong>Q x y</strong> : An order of the commander. Find the height of the highest man among those were standing from position x to position y of the line (1 �� x �� y �� k , k denotes the number of soldiers was currently in the line). </li>
</ul>
</li>
</ul>
<p>&nbsp;</p>
<h3>Output</h3>
<p>The output contains several lines:</p>
<ul>
<li> For each order of the commander, write in one line the number all soldiers had to say loudly. </li>
</ul>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
10
A 1 1
A 2 2
Q 1 2
A 3 1
A 4 3
Q 2 4
A 5 2
Q 2 3
A 6 3
Q 1 4

<strong>Output:</strong>
2
4
5
6
</pre>
<p> </p>