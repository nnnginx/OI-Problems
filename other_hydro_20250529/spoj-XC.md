<p>Xavier, a 9-year-old student, loves playing many kinds of puzzles. One of his favourites is the following:</p>
<p>Xerier, his classmate, has made many cards. She writes down a single positive number on each of them. No numbers written on different cards are the same. After that she writes down an equation, whose right side is a single positive number chosen by her, and the left side is the sum of p integers:</p>
<p><img src="../../../content/john_jones:xc1.jpg" alt=""></p>
<p>Then she asks Xavier put p cards on the corresponding X<sub>i</sub>'s position to make this equation correct, <strong>with an additional condition that X<sub>i</sub> should be ordered from smaller to bigger</strong>, i.e.</p>
<p><img src="../../../content/john_jones:xc2.jpg" alt=""></p>
<p>Every time Xavier immediately comes up with many solutions. Now he wants to know how many solutions in total are there for any n given by Xerier.</p>
<h3>Input</h3>
<p>There are multiple test cases. The number of them is given in the beginning of the input. Then a series of input block comes one by one.</p>
<p>For each test case:</p>
<p>The first line contains two space-separated integers m and p (1&lt;=p&lt;=5). The second line contains m distinct positive integers - the numbers written on each of the cards. None of these integers exceeds 13000.</p>
<p>There are about 120 test cases in total, but 90% of them are relatively small. More precisely, all numbers are less than or equal to 100 in 90% of the test cases.</p>
<h3>Output</h3>
<p>For each test case:</p>
<p>For each positive integer, output the number of ways in a single line. To keep the output finite, only numbers with positive ways should be outputted.</p>
<p>Output a blank line after each test case. See sample for more format details.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
3 3
1 2 3
5 4
1 3 5 6 7
10 3
1 2 3 4 5 6 7 8 9 10

<strong>Output:</strong>
Case #1:
6: 1

Case #2:
15: 1
16: 1
17: 1
19: 1
21: 1

Case #3:
6: 1
7: 1
8: 2
9: 3
10: 4
11: 5
12: 7
13: 8
14: 9
15: 10
16: 10
17: 10
18: 10
19: 9
20: 8
21: 7
22: 5
23: 4
24: 3
25: 2
26: 1
27: 1

</pre>
<p><em>This problem has 82 submissions during the onsite contest, but none of them gets Accepted.</em></p>