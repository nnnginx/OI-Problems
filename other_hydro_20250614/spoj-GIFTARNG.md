<p>Duck's birthday is coming soon! Unfortunately, this year nobody will come to Duck's birthday party. To make himself feel better, he has decided to display all birthday gifts received last year, pretending many people celebrate with him this year.</p>
<p>There are <strong>N</strong> gifts received last year, each in a rectangular gift box with dimensions {<strong>W<sub>i</sub></strong> (width), <strong>H<sub>i</sub></strong> (height), <strong>D<sub>i</sub></strong> (depth)}. Gift box is very colorful which makes people happy, so Duck will place all of them in a straight line without changing the order and without any gap between two adjacent boxes, while the total visible area is maximized. To achieve this goal, Duck can rotate each gift box in any direction but the box must stand upright on the ground. That is, it cannot be placed obliquely. Please help him figure out the largest visible area.</p>
<h3>Input</h3>
<p>The first line is the number of test cases <strong>T</strong>. (1 ¡Ü T ¡Ü 30)</p>
<p>For each test case, it starts with the number of gifts received last year <strong>N</strong>. (1 ¡Ü N ¡Ü 10<sup>3</sup>)</p>
<p>Following N lines, each consisting of three integers <strong>W<sub>i</sub></strong> (width) <strong>H<sub>i</sub></strong> (height) <strong>D<sub>i</sub></strong> (depth), representing the dimensions of the i gift box. (1 ¡Ü Wi, Hi, Di ¡Ü 10<sup>5</sup>)</p>
<h3>Output</h3>
<p>Output the largest visible area.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
2
100 100 20
3 4 2
 
3
1 1 1
5 4 3
8 6 8
</pre>
<pre><strong>Output:</strong>
26032
330
</pre>
<h3>Explanation</h3>
<p>In case 1, one optimal strategy is to rotate the first box to {100, 20, 100} and the second box to {4, 2, 3}.<br> In case 2, no rotation for the first box and third box, and to rotate the second box to {5, 3, 4}.</p>