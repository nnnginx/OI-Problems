<p>Have you ever wondered why people collide with each other at pedestrian crossings? The reasons are probably difficult to analyse from a scientific point of view, but we can hazard a guess. A part of the problem seems to be that the statistical pedestrian, when faced with a red light, will either cross at once (this category of pedestrians doesn't really interest us, since they tend to collide with cars rather than with each other), or will stop dead and stand still until the light changes. Only when the light turns green does he begin to act rationally and heads for his destination using the shortest possible path. Since this usually involves crossing the road slightly on the bias, he will inevitably bump into someone going across and heading another way.
</p><p>
One day, while you are approaching the traffic lights you usually cross at, you begin to wonder how many other people you could possibly collide with if you really wanted. All the people are standing at different points on the same side of the street as you are. From past observations you can predict the exact angle and speed at which individual pedestrians are going to cross. You can decide at which point along the side of the street you will wait for the green light (any real coordinate other than a place where some other pedestrian is already standing) and at what angle and at what speed you intend to cross. There is an upper bound on the speed you may cross at.
</p><p>Assume that once the light turns green, all pedestrians start moving along straight lines, at constant speed, and that collisions, however painful they may be, have no effect on their further progress. Since you wouldn't like to arouse anyone's suspicions, you also have to cross in accordance with these rules. A collision only occurs if at a given moment of time you have exactly the same x and y coordinates as some other pedestrian.

</p><h3>Input</h3>
<p>Input starts with a single integer t, the number of test cases (t&lt;=100). t test cases follow.
</p><p>Each test case begins with a line containing three integers n w v, denoting the number of people other than you who wish to cross the street, the width of the street expressed in meters, and the maximum speed you can walk at given in meters per second, respectively (1&lt;=n&lt;=10000, 1&lt;=w&lt;=100, 1&lt;=v&lt;=10000). Each of the next n lines contains three integers x<sub>i</sub> t<sub>i</sub> a<sub>i</sub>, which describe the starting position of the i-th pedestrian measured in meters, the time (in seconds) he takes to cross the street, and the 
angle at which he is walking with respect to the line normal to the sides of the street, expressed in 1/60 parts of a degree (-10000&lt;=x<sub>i</sub>&lt;=10000, 1&lt;=t<sub>i</sub>&lt;=10000, -5000&lt;=a<sub>i</sub>&lt;=5000).</p>

<img src="/content/adrian:zebra.png" alt="Illustration of problem input">

<h3>Output</h3>
<p>For each test case output a single integer -- the maximum number of people you can collide with by the time you reach the opposite side of the street.

</p><h3>Example</h3>

<pre><b>Input:</b>
1
5 20 2
-20 10 2700
20 10 -2700
-5 1 4000
-4 1 4000
5 1 -4000

<b>Output:</b>
2
</pre>

<p>(In the example, due to the imposed speed limit, it is only possible to collide with the first two pedestrians while crossing the street, at the last possible moment.)
</p>