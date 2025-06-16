<p>Any positive integer v can be written as p<sub>1</sub><sup>a1</sup> ∗ p<sub>2</sub><sup>a2</sup> ∗ . . . ∗ p<sub>n</sub><sup>an</sup> where pi is a prime number and ai ≥ 0. For example: 24 = 2<sup>3</sup> ∗ 3<sup>1</sup> .</p>
<p>Pick any two prime numbers p1 and p2 where p<sub>1</sub> != p<sub>2</sub> . Imagine a two dimensional plane where the powers of p<sub>1</sub> are plotted on the x-axis and the powers of p<sub>2</sub> on the y-axis. Now any number that can be written as p<sub>1</sub><sup>a1</sup> ∗ p<sub>2</sub><sup>a2</sup> can be plotted on this plane at location (x, y) = (a1 , a2 ). The figure on the right shows few examples where p<sub>1</sub> = 3 and p<sub>2</sub> = 2.</p>
<p>This idea can be extended for any N -Dimensional space where each of the N axes is assigned a unique prime number. Each N -Dimensional space has a unique set of primes. We call such set the Space Identification Set or S for short. |S| (the ordinal of S) is N .</p>
<p>Any number that can be expressed as a multiplication of pi ∈ S (each raised to a power (ai ≥ 0) can be plotted in this |S|-Dimensional space. The figure at the bottom illustrates this idea for N = 3 and S = {2, 3, 7}. Needless to say, any number that can be plotted on space A can also be plotted on space B as long as S<sub>A</sub> ⊂ S<sub>B</sub> .</p>
<p>We define the distance between any two points in a given N -Dimensional space to be the sum of units traveled to get from one point to the other while following the grid lines (i.e. movement is always parallel to one of the axes.) For example, in the figure below, the distance between 168 and 882 is 4.</p>
<p>Given two positive integers, write a program that determines the minimum ordinal of a space where both numbers can be plotted in. The program also determines the distance between these two integers in that space.</p>
<p><img src="./21376/file/BRhpscmP.png" alt=""><img src="./21376/file/kwCVVtyH.png" alt=""></p>
<h3>Input</h3>
<p>Your program will be tested on one or more test cases. Each test case is specified on a line with two positive integers (0 &lt; A, B &lt; 1, 000, 000) where A ∗ B &gt; 1.<br>The last line is made of two zeros.</p>
<h3>Output</h3>
<p>For each test case, print the following line:</p>
<p>k. X:D</p>
<p>Where k is the test case number (starting at one,) X is the minimum ordinal needed in a space that both A and B can be plotted in. D is the distance between these two points.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>168 882<br>770 792<br>0 0<br><br><strong>Output:</strong><br>1. 3:4<br>2. 5:6</pre>