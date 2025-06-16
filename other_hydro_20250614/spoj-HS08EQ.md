<p>The definition of a perfect number is about 2300 years old. A perfect number is defined as a positive integer which is the sum of its proper positive divisors, that is, the sum of the positive divisors excluding the number itself. What can we get if,  in the sum,  we replace each divisor by its square? You can prove that there is no such number. But there are many numbers for which the sum of some divisors' squares is equal to <em>n</em>, so n=d<sub>1</sub><sup>2</sup>+d<sub>2</sub><sup>2</sup>+...+d<sub>k</sub><sup>2</sup>, where d<sub>1</sub>, d<sub>2</sub>, ...,d<sub>k</sub> are distinct (positive) divisors of <em>n</em>. You have to count how many times this happens. For example: the divisors of <em>n</em>=120 are 1, 2, 3, 4, 5, 6, 8, 10, 12, 15, 20, 24, 30, 40, 60, 120. And there are exactly two amazing equalities: <br> 120=2<sup>2</sup>+4<sup>2</sup>+10<sup>2</sup> <br> 120=2<sup>2</sup>+4<sup>2</sup>+6<sup>2</sup>+8<sup>2</sup></p>
<h3>Input</h3>
<p>The first number is <em>T</em>, denoting the number of test cases (<em>T</em>&lt;1000). <em>T</em> lines follow, each of which contains one positive integer (<em>n</em>&lt;10<sup>10</sup>).</p>
<h3>Output</h3>
<p>Output <em>T</em> lines, the answer for each <em>n</em>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
6
120
720
1000
1200
92070
123618780

<strong>Output:</strong>
2
13
0
10
6448
292
</pre>