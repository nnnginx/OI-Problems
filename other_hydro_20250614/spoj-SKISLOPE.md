<p>A skier wants to ski down from the top of a mountain to its base. There are several possible routes, using different slopes enroute, and passing through some flat areas. The effort expended in skiing down a slope depends upon the length of the slope and the speed of skiing. For each slope, there is a maximum advisable speed. The skier wants to use a toute that minimizrs the <strong>average effort spent per unit distance traveled</strong> (i.e. the total effort expended divided by the total distance traveled).</p>
<p>The flat regions on the mountain are numbered 1 to N from top to bottom. The skier begins at level 1 and needs to reach level N. You are given the numbers of the flat regions each slope connects. Note that on a slope, one can only ski downwards. For each slope, you are also given the length of the slope and the maximum advisable speed for it. The effort expended in skiing down a particular slope is given by the following formula:</p>
<p>e = d*(70-s) if s ¡Ü 60, and e = d*(s-50) if s &gt; 60</p>
<p>where e is the effort required, d is the distance traveled and s is the speed of travel.</p>
<p>You have to determine the minimum average effort per unit distance that the skier has to expend in order to reach the mountain base, while staying within the maximum advisable speed at every slope.</p>
<h3>Input</h3>
<p>The first line of input gives the number of test cases T(¡Ü20). This is followed by the descriptions of the test cases</p>
<p>For each test case, the first line of input gives the number of flats, N (N ¡Ü 1000), and the number of slopes, R (R ¡Ü 20000), connecting them respectively. Each of the next R lines describes a slope by giving: the numbers of the flats at the top and the bottom of the slope, the maximum advisable speed for the slope (¡Ü 100), and the length of the slope (¡Ü 1000) respectively.</p>
<h3>Output</h3>
<p>For each test case, output a single number (with four places after the decimal point, rounded up) that gives the minimum average effort per unit distance that needs to be expended to ski down from the mountain top to the base. The output for each test case should be on a separate line.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
4 5
1 4 30 60
1 2 50 40
1 3 60 20
2 4 60 50
3 4 50 50
3 3
1 2 50 40
1 3 40 20
2 3 20 30

<strong>Output:</strong>
14.4445
30.0000
</pre>