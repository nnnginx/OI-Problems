<p>There are N cities, numbered from 1 to N,&nbsp;in the country you are living. <strong>Each pair</strong> of the cities is connected with exactly one road. However, <strong>each road is a one-way road</strong>, so it is either possible to go&nbsp;directly from A to B or from B to A for each pair of cities (A, B).</p>
<p>You are living in city #1 and you are practicing for upcoming cycling marathon, so you want to construct the following training plan:</p>
<p>First day you have to ride over 3 roads starting from and finishing in city #1.</p>
<p>Second day you have to ride over 4 roads in the same manner.</p>
<p>Third day you have to ride over 5 roads.</p>
<p>...</p>
<p>The last, (N-2)-th, day you have to ride over N roads starting from and finishing in city #1.</p>
<p>You don't like to visit the same city more than once per day, so you have to find a training route for each day that passes through <strong>each city at most once</strong>. City #1 should appear only at the start and at the end of each route.</p>
<p>Write the program that, given the layout of the network, outputs training route for each day, or writes "impossible" if such training plan is not achievable.</p>
<h3>Input</h3>
<p>The first line of input contains the integer N (3 ¡Ü N ¡Ü 1000), number of cities.</p>
<p>Each of the next N lines contains exactly N characters that describes network layout. <em>j</em>-th character in&nbsp;<em>i</em>-th of these lines is '1' if it is possible to ride from city number <em>i</em> to city number <em>j</em>, or '0' otherwise.</p>
<h3>Output</h3>
<p>You should output training route for each day in a separate line. Training route consists of space separated integers - numbers of the cities in order they should be visited. Each training route starts and ends with 1.</p>
<p>If there is no achievable training plan, output word 'impossible' in a single line, instead.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5
01000
00011
11001
10100
10010

<strong>Output:</strong>
1 2 5 1
1 2 4 3 1
1 2 4 3 5 1
</pre>