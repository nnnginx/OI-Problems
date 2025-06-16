<p>Ada the Ladybug is a farmer. She has a long furrow in which she grows trees. Each tree has some weigth. The task is simple, she wants to know the biggest tree on some part of the furrow which is not greater than some height <strong>H</strong>. As Ada asks for this very often, she asked you to write a program for this.</p>
<h3>Input</h3>
<p>The first line will contain two integer <strong>1 ¡Ü N, Q ¡Ü     3*10<sup>5</sup></strong>, the number trees and the number of questions.</p>
<p>The next line will contain <strong>N</strong> integers <strong>0 ¡Ü A<sub>i</sub> ¡Ü     10<sup>6</sup></strong>, the heights of trees.</p>
<p>The sum next <strong>Q</strong> will contain three integers: <strong> 0 ¡Ü l ¡Ü r &lt;     N</strong>, the segment of furrow she is interested in and <strong>0 ¡Ü H ¡Ü 10<sup>6</sup></strong></p>
<h3>Output</h3>
<p>For each query output either the size of highest tree lesser/equal to <strong>H</strong> or output <strong>0</strong> if such tree doesn't grow on given segment.</p>
<h3>Example Input</h3>
<pre>9 8
1 5 9 11 9 7 6 2 1
1 6 4
1 6 10
0 8 97
0 8 4
1 4 5
2 6 8
2 8 5
3 3 12
</pre>
<h3>Example Output</h3>
<pre>0
9
11
2
5
7
2
11
</pre>