## Description

<div><p>How horrible! The empire of galactic chickens tries to conquer a beautiful city «Z», they have built a huge incubator that produces millions of chicken soldiers a day, and fenced it around. The huge incubator looks like a poligon on the the plane <span class="tex-span"><i>Oxy</i></span> with <span class="tex-span"><i>n</i></span> vertices. Naturally, DravDe can't keep still, he wants to destroy the chicken empire. For sure, he will start with the incubator.</p><p>DravDe is strictly outside the incubator's territory in point <span class="tex-span"><i>A</i>(<i>x</i><sub class="lower-index"><i>a</i></sub>, <i>y</i><sub class="lower-index"><i>a</i></sub>)</span>, and wants to get inside and kill all the chickens working there. But it takes a lot of doing! The problem is that recently DravDe went roller skating and has broken both his legs. He will get to the incubator's territory in his jet airplane LEVAP-41.</p><p>LEVAP-41 flies at speed <span class="tex-span"><i>V</i>(<i>x</i><sub class="lower-index"><i>v</i></sub>, <i>y</i><sub class="lower-index"><i>v</i></sub>, <i>z</i><sub class="lower-index"><i>v</i></sub>)</span>. DravDe can get on the plane in point <span class="tex-span"><i>A</i></span>, fly for some time, and then air drop himself. DravDe is very heavy, that's why he falls vertically at speed <span class="tex-span"><i>F</i><sub class="lower-index"><i>down</i></sub></span>, but in each point of his free fall DravDe can open his parachute, and from that moment he starts to fall at the wind speed <span class="tex-span"><i>U</i>(<i>x</i><sub class="lower-index"><i>u</i></sub>, <i>y</i><sub class="lower-index"><i>u</i></sub>, <i>z</i><sub class="lower-index"><i>u</i></sub>)</span> until he lands. Unfortunately, DravDe isn't good at mathematics. Would you help poor world's saviour find such an air dropping plan, that allows him to land on the incubator's territory? If the answer is not unique, DravDe wants to find the plan with the minimum time of his flight on the plane. If the answers are still multiple, he wants to find the one with the minimum time of his free fall before opening his parachute</p></div><div class="input-specification"><p>The first line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>) — amount of vertices of the fence. Then there follow <span class="tex-span"><i>n</i></span> lines containing the coordinates of these vertices (two integer numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span>) in clockwise or counter-clockwise order. It's guaranteed, that the fence does not contain self-intersections.</p><p>The following four lines contain coordinates of point <span class="tex-span"><i>A</i>(<i>x</i><sub class="lower-index"><i>a</i></sub>, <i>y</i><sub class="lower-index"><i>a</i></sub>)</span>, speeds <span class="tex-span"><i>V</i>(<i>x</i><sub class="lower-index"><i>v</i></sub>, <i>y</i><sub class="lower-index"><i>v</i></sub>, <i>z</i><sub class="lower-index"><i>v</i></sub>)</span>, <span class="tex-span"><i>F</i><sub class="lower-index"><i>down</i></sub></span> and speed <span class="tex-span"><i>U</i>(<i>x</i><sub class="lower-index"><i>u</i></sub>, <i>y</i><sub class="lower-index"><i>u</i></sub>, <i>z</i><sub class="lower-index"><i>u</i></sub>)</span>. All the input numbers are integer. All the coordinates don't exceed <span class="tex-span">10<sup class="upper-index">4</sup></span> in absolute value. It's guaranteed, that <span class="tex-span"><i>z</i><sub class="lower-index"><i>v</i></sub> &gt; 0</span> and <span class="tex-span"><i>F</i><sub class="lower-index"><i>down</i></sub>, <i>z</i><sub class="lower-index"><i>u</i></sub> &lt; 0</span>, and point <span class="tex-span"><i>A</i></span> is strictly outside the incubator's territory.</p></div><div class="output-specification"><p>In the first line output two numbers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub></span> such, that if DravDe air drops at time <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span> (counting from the beginning of the flight), he lands on the incubator's territory (landing on the border is regarder as landing on the territory). If DravDe doesn't open his parachute, the second number should be equal to the duration of DravDe's falling down. If it's impossible for DravDe to get to the incubator's territory, output <span class="tex-font-style-tt">-1 -1</span>. If the answer is not unique, output the answer with the minimum <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span>. If the answers are still multiple, output the answer with the minimum <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span>. Your answer must have an absolute or relative error less than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>


## Input

<p>The first line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>) — amount of vertices of the fence. Then there follow <span class="tex-span"><i>n</i></span> lines containing the coordinates of these vertices (two integer numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span>) in clockwise or counter-clockwise order. It's guaranteed, that the fence does not contain self-intersections.</p><p>The following four lines contain coordinates of point <span class="tex-span"><i>A</i>(<i>x</i><sub class="lower-index"><i>a</i></sub>, <i>y</i><sub class="lower-index"><i>a</i></sub>)</span>, speeds <span class="tex-span"><i>V</i>(<i>x</i><sub class="lower-index"><i>v</i></sub>, <i>y</i><sub class="lower-index"><i>v</i></sub>, <i>z</i><sub class="lower-index"><i>v</i></sub>)</span>, <span class="tex-span"><i>F</i><sub class="lower-index"><i>down</i></sub></span> and speed <span class="tex-span"><i>U</i>(<i>x</i><sub class="lower-index"><i>u</i></sub>, <i>y</i><sub class="lower-index"><i>u</i></sub>, <i>z</i><sub class="lower-index"><i>u</i></sub>)</span>. All the input numbers are integer. All the coordinates don't exceed <span class="tex-span">10<sup class="upper-index">4</sup></span> in absolute value. It's guaranteed, that <span class="tex-span"><i>z</i><sub class="lower-index"><i>v</i></sub> &gt; 0</span> and <span class="tex-span"><i>F</i><sub class="lower-index"><i>down</i></sub>, <i>z</i><sub class="lower-index"><i>u</i></sub> &lt; 0</span>, and point <span class="tex-span"><i>A</i></span> is strictly outside the incubator's territory.</p>


## Output

<p>In the first line output two numbers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub></span> such, that if DravDe air drops at time <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span> (counting from the beginning of the flight), he lands on the incubator's territory (landing on the border is regarder as landing on the territory). If DravDe doesn't open his parachute, the second number should be equal to the duration of DravDe's falling down. If it's impossible for DravDe to get to the incubator's territory, output <span class="tex-font-style-tt">-1 -1</span>. If the answer is not unique, output the answer with the minimum <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span>. If the answers are still multiple, output the answer with the minimum <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span>. Your answer must have an absolute or relative error less than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>


## Samples

```input1
4
0 0
1 0
1 1
0 1
0 -1
1 0 1
-1
0 1 -1

```

```output1
1.00000000 0.00000000

```






```input2
4
0 0
0 1
1 1
1 0
0 -1
-1 -1 1
-1
0 1 -1

```

```output2
-1.00000000 -1.00000000

```






```input3
4
0 0
1 0
1 1
0 1
0 -1
1 1 1
-1
1 1 -1

```

```output3
0.50000000 0.00000000

```



