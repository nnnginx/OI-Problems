<p>Christy C. Coder is traveling to Waterloo for a programming competition. On the way, she stops in Toronto to do some sightseeing. The unfortunate thing about travelling is that everyone back home expects her to bring back pictures of everything. Christy hates taking pictures: it makes her look like such a tourist! Fortunately, Christy has a plan to make her picture-taking quite painless.</p>
<p>At 553 m tall, CN Tower is the world's tallest free-standing building. 351 m up the tower is the "360" rotating restaurant, which rotates a full 360 degrees every 72 minutes. From there, Christy can see the whole city, and take close-up pictures of all the landmarks using her fancy new 100x optical zoom camera. Since the restaurant itself rotates, she only needs to stand in one place to take pictures in all directions.</p>
<p>The waiters insist that she order something or leave, and Christy is not interested in any of the items on the menu. Therefore, she must act quickly before she gets kicked out. Given the locations of the landmarks of which Christy wants to take a picture, your task is to determine the minimum amount of time that she must spend in the restaurant in order for it to rotate enough to bring all the landmarks in view. Assume that Christy always points her camera exactly perpendicular to the window to minimize distortion due to the glass. Note that multiple landmarks may occupy the same (angular) position, and these landmarks would only require one photograph to capture them.</p>
<p>Since the restaurant staff only realize she is a tourist once she starts taking pictures, we begin measuring the time required once she takes her first picture. Therefore, Christy can move to any position in the restaurant without hassle from the restaurant staff and begin taking pictures from there.</p>
<h3>Input</h3>
<p>The first line of input consists of the number of test cases. For each test case, the first line is an integer <em>n</em> (2 ¡Ü <em>n</em> ¡Ü 1000), the number of landmarks Christy wants to photograph. Each of the following <em>n</em> lines specify a landmark. Each landmark specification consists of the landmark name (a string of uppercase and lowercase letters of length at most 40 characters), a space, and the compass angle <em>d</em>, in degrees, to the landmark from the CN Tower (0 = north, 90 = east, 180 = south, 270 = west). Note that <em>d</em> is a real number which satisfies 0 ¡Ü <em>d</em> &lt; 360, with <em>d</em> specified to the hundredth of a degree (i.e., at most two decimal places).</p>
<h3>Output</h3>
<p>For each test case, output a single integer, the minimum number of seconds that Christy must remain in the restaurant. If the time is not an integer number of seconds, round it up to the nearest second (i.e., take the ceiling of the number).</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
5
CasaLoma 231.0
OntarioParliament 123.0
SkyDome 75.0
RoyalYorkHotel 340.0
PearsonAirport 165.0

<strong>Output:</strong>
3012</pre>