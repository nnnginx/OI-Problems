<p>Johnny is playing with some dominoes one afternoon. His dominoes come in a variety of heights and colors.<br> <br> Just like any other child, he likes to put them in a row and knock them over.<br> He wants to know something: how many pushes does it take to knock down all the dominoes?<br> Johnny is lazy, so he wants to minimize the number of pushes he takes.<br> A domino, once knocked over, will knock over any domino that it touches on the way down.<br> <br> For the sake of simplicity, imagine the floor as a one-dimensional line, where 1 is the leftmost point. Dominoes will not slip along the floor once toppled. Also, dominoes do have some width: a domino of length 1 at position 1 can knock over a domino at position 2. <br> For the mathematically minded:<br> A domino at position <em>x</em> with height <em>h</em>, once knocked over to the right, will knock all dominoes at positions <em>x</em>+1, <em>x</em>+2, ..., <em>x</em>+<em>h</em> rightward as well.<br> Similarly, the same domino knocked over to the left will knock all dominoes at positions <em>x</em>-1, <em>x</em>-2, ..., <em>x</em>-<em>h</em> leftward.</p>
<h3>Input</h3>
<p>The input starts with a single integer <em>N</em> (<em>N</em> ¡Ü 100000), the number of dominoes, followed by <em>N</em> pairs of integers.<br> Each pair of integers represents the location and height of a domino, in that order (0 ¡Ü location ¡Ü 10<sup>9</sup>, 0 ¡Ü height ¡Ü 10<sup>9</sup>).<br> No two dominoes will have the same location.</p>
<h3>Output</h3>
<p>A single integer on a single line: the minimum number of pushes Johnny must make in order to ensure that all dominoes are knocked over.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
6
1 1
2 2
3 1
5 1
6 1
8 3
<strong>Output:</strong>
2
<strong>Explanation</strong>
              |
  |           |
| | |   | |   |
1 2 3 4 5 6 7 8
</pre>
<p>Pushing 1 causes 2 and 3 to fall, while pushing 8 causes 6 to fall and gently makes 5 tip over as well.</p>