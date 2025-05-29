<p><em>Original statement in spanish at <a href="http://www.dc.uba.ar/events/icpc/download/problems/taip2011-problems.pdf">http://www.dc.uba.ar/events/icpc/download/problems/taip2011-problems.pdf</a></em></p>
<p>The mean and the median usually confuse the students because of their similar spelling, but they are quite different concepts. In this problem we are going to work with the mean and the median of a set consisting of <strong>N</strong> pairwise distinct integers, where <strong>N</strong> is odd. The mean of such set is defined, as usual, as the sum of the numbers divided by <strong>N</strong>, while the median is the unique element in the set that is greater than (<strong>N</strong>-1)/2 of its elements, and less than the other (<strong>N</strong>-1)/2 elements in the set. For instance, if the set is {0, 2, 6, 4, 13}, then the mean is 5 while the median is 4.</p>
<p>We aim to make student's lives easier by generating "balanced" sets, that is, sets consisting of an odd number of pairwise distinct integers where the mean and the median coincide. For example, the set {0, 2, 6, 4, -2} is balanced, since it has <strong>N</strong>=5 different integers, and the mean and the median are both equal to 2.</p>
<p>The following procedure has been suggested in order to obtain balanced sets. A set with an even number of distinct integers is chosen, and an extra integer distinct from every element in the set is added to it, in such a way that the resulting set is balanced. We want you to check if the given procedure works. Therefore your task is, given <strong>N</strong>-1 distinct integers, with odd <strong>N</strong>, count the number of balanced sets that can be formed by following the described procedure.</p>
<h3>Input</h3>
<p>The input contains several test cases. Each test case is described with two lines. The first line contains a single odd positive integer <strong>N</strong> that indicates the number of elements the balanced set must have (3 &lt;= <strong>N</strong> &lt;= 499). The second line contains <strong>N</strong>-1 distinct integers <strong>Z_i</strong> that represent the given elements of the set (-10<sup>14</sup> &lt;= <strong>Z_i</strong> &lt;= 10<sup>14</sup> for 1 &lt;= <strong>i</strong> &lt;= <strong>N</strong>-1). The last line of the input contains the number -1, and should not be processed as a test case.</p>
<h3>Output</h3>
<p>For each test case, output a single line with an integer representing the total number of different balanced sets that can be obtained by adding an integer to the given set, as explained in the problem description.</p>
<h3>Example</h3>
<p><strong>Input:</strong></p>
<pre>5
0 2 6 4
7
1 2 3 4 5 8
3
-100000000000000 100000000000000
-1
</pre>
<p><strong>Output:</strong></p>
<pre>3
1
3
</pre>