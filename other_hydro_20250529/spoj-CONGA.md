<p>Conga is a traditional dance in which people make a line, grab each other by the waist and start dancing around.</p>
<p>You are at a party and your favorite Conga song starts playing. Since you want to make the most of it, you'd like to organize everybody and start dancing as soon as possible.</p>
<p>The dance floor is modeled as an infinite straight line with people standing on positive integer coordinates. There is at most one person at each point. Every second, a person can move one unit to the left or one unit to the right, as long as no one else is standing there. However, since it's a crazy party and people are already drunk, at most one person can move every second (in other words, no two people can move simultaneously).</p>
<p>Nobody will start dancing until everybody is organized in a perfect line. You want to find the minimum amount of time it takes to start dancing, i.e. the time it takes to make people stand in such a way that there are no empty spaces between them.</p>
<p>For example, imagine there are 4 people at the party, standing at positions 2, 4, 5 and 8:</p>
<p><img src="./21925/file/YZ7EMFLI.png" alt="Conga line" width="966" height="165"></p>
<p>In this case, it takes at least 3 seconds to form the Conga line:</p>
<ul>
<li>On second 1, the person standing at position 2 moves to position 3.</li>
<li>On second 2, the person standing at position 8 moves to position 7.</li>
<li>On second 3, the person standing at position 7 moves to position 6.</li>
<li>After three seconds, people are standing on positions 3, 4, 5, and 6 and they can start dancing!</li>
</ul>
<p><img src="./21925/file/6J327igM.png" alt="Start dancing" width="974" height="165"></p>
<h3>Input</h3>
<p>The input contains several test cases.</p>
<p>The first line of each case contains a single integer number <em>n</em>, the number of people in the party (1 ¡Ü <em>n</em> ¡Ü 10<sup>6</sup>). The next line contains <em>n</em> distinct integers x<sub>i</sub> separated by single spaces sorted in ascending order ¡ª the coordinates where people are initially standing (1 ¡Ü <em>x<sub>i</sub></em> ¡Ü 10<sup>9</sup>).</p>
<p>The last line of the input contains a single <em>0</em> and should not be processed.</p>
<h3>Output</h3>
<p>For each test case, output one integer number on a single line ¡ª the minimum time it takes to start dancing.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4<br>2 4 5 8<br>1<br>10<br>4<br>20 24 25 26<br>2<br>1 2<br>2<br>1 1000000000<br>0

<strong>Output:</strong>
3<br>0<br>3<br>0<br>999999998
</pre>