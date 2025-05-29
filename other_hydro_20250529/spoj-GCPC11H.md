<p>As a computer science student you are of course very outdoorsie, so you decided to go hiking. For your vacation this year, you located an island full of nice places to visit. You already identified a number of very promising tracks, but are still left with some problems. The number of choices is so overwhelming, that you had to select only a "small" subset of at most <em>10<sup>5</sup></em> sights.</p>
<p>And if that is not enough, you are very picky about the order in which you want to visit the sights. So you have already decided on an order in which you want to visit the preselected tracks. The problem you are left with is to decide in which direction to travel along each single track, and whether you may have to reduce your choice of tracks even further. After identifying the travel time between the endpoints of different tracks, you decide to write a program to figure out if you can make all your trips within the time you have planned for your vacation. Since you also do not want to waste any precious time, you only care about an optimal solution to your problem. Furthermore, the tracks can get pretty challenging. Thats why you do not want to hike along a track more than once.</p>
<h3>Input</h3>
<p>The first line of the input gives the number of test cases <em>C</em> (<em>0 &lt; C ¡Ü 100</em>). The first line of each such test case holds two integers <em>N</em>, <em>T</em> the number of tracks of the current hiker (<em>1 ¡Ü N ¡Ü 10<sup>5</sup></em>) and the maximal time spent hiking throughout the vacation (<em>0 ¡Ü T ¡Ü 10<sup>6</sup></em>). Each of the following <em>N</em> lines holds five integers <em>c<sub>p</sub></em>, <em>c<sub>bb</sub></em>, <em>c<sub>be</sub></em>, <em>c<sub>eb</sub></em> and <em>c<sub>ee</sub></em> that describe a track (in order of importance). <em>c<sub>p</sub></em> gives the length of the track in minutes. <em>c<sub>xy</sub></em> gives the travel time of the official <strong>b</strong>egin or <strong>e</strong>nd of a track to the <strong>b</strong>eginning or <strong>e</strong>nd of the next most important track, where <em>x</em> and <em>y</em> are either <em>b</em> or <em>e</em>. All values given are non-negative integers not greater than <em>10<sup>6</sup></em>. Since you have to get back to your car, the list is circular. Furthermore, we will ignore the time it takes you to get to the start of your trip with your car.</p>
<h3>Output</h3>
<p>For each test case print one line. The output should contain a list of either <strong>F</strong> or <strong>B</strong> for every track (in order) indicating whether you have to hike the track in forward direction or backward direction. If you cannot make the full trip within the planned time <em>T</em>, you should print <strong>IMPOSSIBLE</strong> to indicate that these trips are just too much hiking. You can assume that the optimal solution is always unique.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
2 100
4 7 8 2 3
1 4 6 1 2
2 20
4 2 3 7 8
1 1 2 4 6
3 5
1 2 2 2 1
1 1 2 2 2
1 2 2 1 2

<strong>Output:</strong>
FF
BB
IMPOSSIBLE
</pre>