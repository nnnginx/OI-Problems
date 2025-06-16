<p>A three-headed monkey was on his (theirs?) peaceful way from his dorm to the university. He decided to use the subway. But as soon as he descended into the station, he was stopped by a strange geek with a flashlight, saying strange words...</p> 

<p><i>"I am a servant of the Secret Group Order, wielder of the flame of Primes. Your limited knowledge of partial derivatives will not avail you, flame of Riemann! You shall not pass! You can't beat Kruskal in his game!" </i></p>

<p>The three-headed monkey shook his head. The left one. But there was no way out. If he wanted to get to the university in time, he had to play. </p>

<p>(Many others in his situation would use the distract-and-run tactics to get past the evil Kruskal into the subway. However, this was not possible in this case : nobody will turn around upon hearing <i>"Hey! Look behind you! A three-headed monkey!"</i> when he already sees the monkey in front of him...) </p>

<p>So, what was the game about? It is a two-player game. At the beginning there are <b>N</b> (not necessarily equal) heaps of matches. On each turn, a player may only remove matches from one heap only, and he has to remove between 1 and <b>K</b> matches, inclusive. A player wins if after his move the size of some heap is a prime number. The three-headed monkey moves first. </p>

<h3>Problem specification</h3>
<p>You will be given several starting positions. For each of them, determine whether the three-headed monkey can win this game. You may assume that Kruskal (the monkey's opponent) plays optimally. </p>

<h3>Input specification</h3>
<p>The first line of the input file contains an integer <b>T</b> specifying the number of test cases. </p>

<p>Each test case looks as follows: on the first line there are the two integers <b>N</b>(1&lt;= <b>N</b> &lt;=200) and <b>K</b>(1&lt;= <b>K</b> &lt;=100), separated by a single space. <b>N</b> lines follow, one for each heap of matches. The <b>i</b>-th of these lines contains a single integer <b>a<sub>i</sub></b>(3&lt;= <b>a<sub>i</sub></b> &lt; 2<sup>32</sup>) giving the number of matches on the <b>i</b>-th heap. </p>

<h3>Output specification</h3>
<p>For each test case output one line. If the monkey can win the game, output the string "YES", otherwise output the string "NO". </p>

<h3>Example</h3>
<pre><b>Input:</b>
2

3 3
48
15
4

2 3
51
51

<b>Output:</b>
YES
NO
</pre>
<b>Note: a somewhat hard <a href="http://www.spoj.com/content/john_jones:kruskal.txt">test</a> has been removed.</b>