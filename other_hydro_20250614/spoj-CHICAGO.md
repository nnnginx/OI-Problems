<p>In the movie "Blues Brothers", the orphanage where Elwood and Jake were raised may be sold to the Board of Education if they do not pay 5000 dollars in taxes at the Cook County Assessor's Office in Chicago. After playing a gig in the Palace Hotel ballroom to earn these 5000 dollars, they have to find a way to Chicago. However, this is not so easy as it sounds, since they are chased by the Police, a country band and a group of Nazis. Moreover, it is 106 miles to Chicago, it is dark and they are wearing sunglasses.<br> As they are on a mission from God, you should help them find the safest way to Chicago. In this problem, the safest way is considered to be the route which maximises the probability that they are not caught.</p>
<h3>Input Specification</h3>
<p>The input file contains several test cases.<br> Each test case starts with two integers <em>n</em> and <em>m</em> (<em>2 �� n �� 100</em> , <em>1 �� m �� n*(n-1)/2</em>). <em>n</em> is the number of intersections, <em>m</em> is the number of streets to be considered.<br> The next <em>m</em> lines contain the description of the streets. Each street is described by a line containing 3 integers <em>a</em>, <em>b</em> and <em>p</em> (<em>1 �� a, b �� n</em> , <em>a �� b</em>, 1 �� p �� 100): <em>a</em> and <em>b</em> are the two end points of the street and <em>p</em> is the probability in percent that the Blues Brothers will manage to use this street without being caught. Each street can be used in both directions. You may assume that there is at most one street between two end points. <br> The last test case is followed by a zero.</p>
<h3>Output Specification</h3>
<p>For each test case, calculate the probability of the safest path from intersection <em>1</em> (the Palace Hotel) to intersection <em>n</em> (the Honorable Richard J. Daley Plaza in Chicago). You can assume that there is at least one path between intersection <em>1</em> and <em>n</em>.<br> Print the probability as a percentage with exactly 6 digits after the decimal point. The percentage value is considered correct if it differs by at most 10<sup>-6</sup> from the judge output. Adhere to the format shown below and print one line for each test case.</p>
<h3>Sample Input</h3>
<pre>5 7
5 2 100
3 5 80
2 3 70
2 1 50
3 4 90
4 1 85
3 1 70
0
</pre>
<h3>Sample Output</h3>
<pre>61.200000 percent
</pre>
<hr>
<p><em>The safest path for the sample input is 1 -&gt; 4 -&gt; 3 -&gt; 5</em></p>