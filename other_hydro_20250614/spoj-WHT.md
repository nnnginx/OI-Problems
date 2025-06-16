<p>A group of <strong>f</strong> friends get together to have a coding problem-solving party at their university computer lab every weekend. Unfortunately, it closes at 22:00, at which point they have no other option but to walk home. The city they live in can be described as <strong>n</strong> junctions connected by <strong>m</strong> bidirectional roads. Since these friends have been interrupted from coding their solutions, each one of them wants to get home as fast as possible to finish his and submit it. At the same time, they each have a few problems that they want to discuss with the others, so they will pick such a path that the entire group can walk together for as long as possible. On top of that, so that this walk would feel fresh every time, they would like to take a different path each weekend, for as long as possible.&nbsp;</p>
<p>The group of friends were able to figure out both the length of the longest path they could all efficiently walk together, as well as how many distinct such paths there are - do you think you can do it, too?</p>
<h3>Input</h3>
<p>The first line contains an integer <strong>T</strong>&nbsp;- the number of test cases. <strong>T</strong>&nbsp;test cases follow, each in the given format. Test cases are separated by a blank line.</p>
<p>The first line of a case contains four integers <strong>n m c f</strong>&nbsp;- the number of junctions, the number of two-way roads connecting the junctions, the junction at which the <strong>c</strong>omputer lab is located, and the number of <strong>f</strong>riends. Junctions are numbered from <strong>1</strong> to <strong>n</strong>.</p>
<p>The second line contains <strong>f</strong>&nbsp;distinct integers <strong>F</strong><sub><strong>1</strong>&nbsp;</sub>, ... ,<strong>F<sub>f</sub></strong>&nbsp;- <strong>F<sub>i</sub>&nbsp;</strong>is the junction where friend number <strong>i</strong>&nbsp;lives. None of them are equal to <strong>c</strong>.</p>
<p>The following <strong>m</strong>&nbsp;lines contain three integers <strong>x y z</strong>, denoting a two-way road connecting junctions <strong>x </strong>and <strong>y</strong>, of length <strong>z. </strong>Each unordered pair <strong>x,y </strong>will be present at most once.</p>
<p>You can assume that the city is connected.</p>
<h3>Output</h3>
<p>Output two integers <strong>L </strong>and <strong>W</strong>.</p>
<p>A 'path' is a sequence of junctions <strong>a<sub>1</sub></strong><strong>&nbsp;...&nbsp;</strong><strong>a</strong><sub><strong>k</strong></sub>where for all <strong>1 </strong><strong>¡Ü i &lt; k</strong>&nbsp;the junctions <strong>a</strong><sub><strong>i</strong> </sub>and<strong> </strong><strong>a</strong><sub><strong>i+1</strong></sub><sub> </sub>are connected by a road<strong>.</strong></p>
<p><strong>L</strong>&nbsp;is the length of the longest path, such that for all <strong>1 ¡Ü i ¡Ü f&nbsp;</strong>if after walking this path friend number <strong>i</strong>&nbsp;can get home the soonest at some time <strong>L</strong>+<strong>t<sub>i</sub></strong>, there exists no path from <strong>c</strong>&nbsp;to <strong>F<sub>i</sub>&nbsp;</strong>shorter than <strong>L</strong>+<strong>t</strong><sub><strong>i</strong></sub>. In other words, none of the friends could have gotten home sooner if they would have chosen a different path which did not include the one of length <strong>L</strong>.</p>
<p><strong>W </strong>is the number of such paths, modulo <strong>10<sup>9</sup>+7</strong>.</p>
<p>Two paths are considered distinct if either</p>
<p>a) they contain a different number of junctions</p>
<p>or</p>
<p>b) they contain the same number of junctions (lets call that&nbsp;<strong>k</strong>), where one path is described by <strong>a<sub>1</sub></strong>&nbsp;... <strong>a</strong><sub><strong>k</strong> </sub>and the other by <strong>b</strong><strong><sub>1</sub></strong>&nbsp;... <strong>b</strong><sub><strong>k</strong>,&nbsp;</sub>and there exists some <strong>1 </strong><strong>¡Ü&nbsp;</strong><strong>i </strong><strong>¡Ü k</strong>&nbsp;such that <strong>a</strong><sub><strong>i</strong> </sub><strong>¡Ù b</strong><sub><strong>i</strong></sub>.</p>
<h3><span style="font-weight: bold;">Constraints</span></h3>
<p><strong>1 &nbsp;<strong>¡Ü f &lt; n <strong>¡Ü 5000</strong></strong></strong></p>
<p><strong>n-1&nbsp;¡Ü m </strong><strong>¡Ü min(10<sup>6</sup>, n*(n-1)/2</strong><strong>&nbsp;)</strong></p>
<p><strong>1 <strong>¡Ü c <strong>¡Ü n</strong></strong></strong></p>
<p><strong>1 <strong>¡Ü F<sub>i&nbsp;</sub><strong>¡Ü n</strong></strong></strong></p>
<p><strong>1 <strong>¡Ü x &lt; y <strong>¡Ü n</strong></strong></strong></p>
<p><strong><strong><strong>1 <strong>¡Ü z <strong>¡Ü 4*10<sup>5</sup></strong>&nbsp;</strong></strong></strong></strong></p>
<p><strong>1 <strong>¡Ü T <strong>¡Ü 500</strong></strong></strong></p>
<p>Additionally, if <strong>T &gt; 1</strong>, <strong>n ¡Ü 50</strong>.</p>
<p>The largest input file is under&nbsp;<strong>16MB</strong>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
9 12 2 3
9 8 1
2 5 3
2 3 7
2 4 5
3 6 4
6 7 2
5 7 20
4 7 8
4 8 50
7 9 10
7 8 30
1 8 15
1 9 15

9 12 2 3
9 8 1
2 5 3
2 3 7
2 4 5
3 6 4
6 7 2
5 7 20
4 7 8
4 8 10
7 9 10
7 8 30
1 8 15
1 9 15

9 12 2 3
9 8 1
2 5 3
2 3 7
2 4 5
3 6 4
6 7 2
5 7 20
4 7 8
4 8 10
7 9 10
7 8 30
1 8 4
1 9 4

<strong>Output:</strong>
13 2
5 1
15 1</pre>
<h4>Explanation</h4>
<p>In the first case, the paths are 2,3,6,7 and 2,4,7. Friends number 1 and 2 can then go straight home, and friend number 3 can go home either through junction 8 or 9. For each friend, this is an optimal path.</p>
<p>In the second case, friend number 1 can get home the fastest the same ways as before, friend number 2 can get home fastest by going 2,4,8 and friend number 3 by going 2,4,8,1. Hence the longest path which all friends are willing to take is 2,4 of length 5, and no other such path exists.</p>
<p>In the third case, the first friend can get home the fastest by 2,3,6,7,9 or 2,4,7,9 or 2,4,8,1,9; the second friend's only fastest path is 2,4,8, and the third friend is only willing to take the path 2,4,8,1. Hence the longest path they are all willing to take has length 15 and it is 2,4,8.&nbsp;</p>