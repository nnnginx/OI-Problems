<p>N(N &lt;= 120) friends decided to go to the local cinema together. They all bought tickets to the same row. As there was still some time left, each of them took her ticket and went shopping until the movie starts.</p>
<p>They all arrived back late, the movie already started. The usher standing at the door agreed to let them in one by one. Each of the girls was supposed to find her place and sit down.</p>
<p>However, the machine that printed their tickets was broken. Instead of consecutive numbers, each girl received a random seat number between 1 and K, where K is the number of seats in their row. The seat numbers they received were not necessarily distinct.</p>
<p>When a girl tries to sit down, she enters the row at the end where seat number 1 is, and walks until she reaches the number on her ticket. If her desired seat is free, she just sits down. If it is already taken, she continues to walk in the same direction until she finds the first free seat, and sits there.</p>
<p>Of course, it is possible that some unfortunate girl will reach the end of the row without finding a place to sit. In that case, the usher comes and throws her out.</p>
<h3>Problem specification</h3>
<p>You are given the numbers N and K.(1&lt;= K &lt;=200)</p>
<p>Assume that each girl's ticket had a number between 1 and K, inclusive. Each number was drawn uniformly at random, and draws were independent.</p>
<p>Also assume that the entire row was empty when the first girl started to look for her seat.</p>
<p>Compute the probability that at least one girl suffered the sad fate of being thrown out by the usher.</p>
<h3>Input specification</h3>
<p>The first line of the input file contains an integer T specifying the number of test cases. Each test case is preceded by a blank line.</p>
<p>Each test case consists of a single line containing two integers N and K.</p>
<h3>Output specification</h3>
<p>For each test case output a single line with the probability as a simplest fraction. (Do not output any spaces before or after the / sign.)</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3

1 10

2 3

3 3

<strong>Output:</strong>
0/1
1/9
11/27
</pre>
<p>In the third case there are 3<sup>3</sup> = 27 possibilities. Out of these, in 11 some girl is thrown out. These 11 sequences are: 133, 222, 223, 232, 233, 313, 322, 323, 331, 332, and 333.</p>
<p>For example, if the sequence of numbers were 322, the first girl sits at seat #3, the second one at #2, and then the third one tries to sit at #2, but finds both seat #2 and seat #3 occupied, and she's thrown out.</p>