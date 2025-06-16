<p>Jane and Tarzan have got cellphones and now they want to be available all the time. They live in a long line of trees and they are available iff the absolute difference between the heights of the two trees which they are on is not greater than D.</p>
<p>Jane and Tarzan are moving by the following rules: each second both Jane and Tarzan (simultaneously) jump, from the tree which they are on, on one of the adjacent trees (the left or the right one). It is forbidden to stay on the same tree. Moreover, in the very beginning and after each second they have to be available.</p>
<p>The trees in the line are numbered from 1 to N, respectively. Jane is interested in the pairs of trees (J, T) �C let's call them good pairs �C for which it holds: if Jane begins on the J-th tree, and Tarzan on the T-th tree, they can swap their positions after some time (moving by the rules) �C so that Tarzan ends on the J-th tree, and Jane on the T-th tree.</p>
<p>Have a look on the first test example. D = 0 means that the heights of the trees which Jane and Tarzan are on have to differ by at most 0 (therefore, have to be equal) all the time. Pair (1, 5) is a good pair since we can take 1-2-3-4-5-6-5 as Jane's route, and 5-6-5-4-3-2-1 as Tarzan's route �C this results in Jane and Tarzan swapping their initial positions (and being available all the time).</p>
<p>Output all the good pairs (J, T) in which J &lt; T.</p>
<h3>Input</h3>
<p>In the first line of input there are integers N (1 �� N �� 100 000) and D (0 �� D �� 10<sup>9</sup>).</p>
<p>In the next N lines there are N natural numbers less than 10<sup>9</sup> �C heights of the trees in the line (from the 1st tree to the N-th tree).</p>
<h3>Output</h3>
<p>Output all the requested pairs in sorted order. We define a pair (A, B) to be smaller than the pair (C, D) iff (A &lt; C) or (A = C and B &lt; D).</p>
<p>In all of the test data, the number of these pairs will not exceed 100 000.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
6 0
2
1
2
3
2
1

<strong>Output:</strong>
1 3
1 5
2 6
3 5
</pre>
<pre><strong>Input:</strong>
5 10
10
20
10
5
10

<strong>Output:</strong>
1 2
1 3
1 4
2 3
2 5
3 4
3 5
4 5
</pre>