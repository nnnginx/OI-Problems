<p>"Holiday is coming, holiday is coming, hurray hurray!" shouts Joke in the last day of his college. On this holiday, Joke plans to go to his grandmother's house located in Schematics village. Joke's grandmother's house is more than a hundred years old. Joke is very kind hearted, so he wants to help renovate the house by painting the fence. The fence consists of N vertical boards placed on a line. The boards are numbered 1 to N from left to right, and each of them has the length of 1 meter and the height of Ai meters.&nbsp;</p>
<p>Joke's grandmother has a paintbrush that can be used to paint the fence. That paintbrush has a length of 1 meter. Joke paints the fence by brushing either horizontally or vertically, but the paint is expensive so Joke wants to minimize the number of paintbrush stroke. On each stroke, the paintbrush will make either a horizontal or vertical line. Also, the paintbrush must be touching the fence for the entire duration of the stroke. Joke also does not want to paint previously panted segment before. Help Joke to find the minimum number of stroke until the entire fence is covered with paint.</p>
<h3>Input</h3>
<p>First line contains a number N, the number of boards on the fence. The second line contains N numbers, A<span style="vertical-align: sub;">1</span>, A<span style="vertical-align: sub;">2</span>, A<span style="vertical-align: sub;">3</span> ... A<span style="vertical-align: sub;">n</span> representing the height of each board.</p>
<h3>Output</h3>
<p>Minimum number of stroke to paint the entire fence.</p>
<h3>Sample Input 1</h3>
<pre>5
2 2 1 2 1</pre>
<h3>Sample Output 1</h3>
<pre>3
</pre>
<h3>Sample Input 2</h3>
<pre>2
2 2</pre>
<h3>Sample Output 2</h3>
<pre>2
</pre>
<h3>Sample Input 3</h3>
<pre>1
5</pre>
<h3>Sample Output 3</h3>
<pre>1</pre>
<div style="border: 1px solid #ADC; background-color: #0cc; padding: 5px; margin-bottom: 10px;">
<h3>Explanation</h3>
<ul>
<li>On the first example, first stroke is done horizontally on the lowest segment. Second stroke is done horizontally on board 1 and board 2 on 2 meters height. Third and last stroke is done on board 4 on 2 meters height, doesn't matter horizontally or vertically.&nbsp;</li>
<li>On the second exapmle, Joke can do either 2 horizontal strokes or 2 vertical strokes.</li>
<li>On the third example, only 1 vertical stroke is needed.</li>
</ul>
</div>
<div style="border: 1px solid #FC0; background-color: #ffc; padding: 5px; margin-bottom: 10px;">
<h3>Constraint</h3>
<ul>
<li>1 ¡Ü N ¡Ü 5000</li>
<li>1 ¡Ü A<span style="vertical-align: sub;">i</span> ¡Ü 1000000000</li>
</ul>
</div>