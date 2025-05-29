<p>Bob is sitting at home with his computer. He would like to experience more social interaction, so he is planning a trip to a coffee shop with his computer.</p>
<p>Bob has lots of data about wireless networks and coffee shops in the city. In Bob��s city, there is one coffee shop at every intersection of streets. Specifically, Bob happens to live in a city with <em>M</em> streets (1 �� <em>M</em> �� 30000) that run east and west, and <em>N</em> streets (1 �� <em>N</em> �� 1000) that run north and south. As an added benefit, the distance between consecutive parallel streets is 1 metre (it is a very compact city).</p>
<p>It also turns out that inside <em>K</em> (1 �� <em>K</em> �� 1000) of the coffee shops, there is a wireless network station. Each wireless network station will have a particular bitrate <em>B</em> (1 �� <em>B</em> �� 1000) and can reach <em>R</em> metres (1 �� <em>R</em> �� 30000) from the coffee shop. In other words, a wireless network station from one coffee shop forms a circle with radius <em>R</em> centered at that particular coffee shop. Moreover, if someone is at distance <em>R</em>, the wireless network would be available, but if someone is at a distance larger than <em>R</em>, they cannot access that wireless point.</p>
<p>You can assume that each coffee shop has at most one wireless network stationed in it, but that multiple wireless networks may be available while sitting in that one coffee shop, due to the proximity of other wireless network stations.</p>
<p>Bob has a special device in his computer that can use all of the available bitrates of as many wireless networks as he can connect to.</p>
<p>Bob would like to find out the maximum bitrate he can obtain, and how many coffee shops would have that maximum capacity.</p>
<h3>Input</h3>
<p>On the first line of input, you will be given the integer <em>M</em>, the number of east-west streets. On the second line of input, you will be given the integer <em>N</em>, the number of north-south streets. On the third line of input, you will be given the integer <em>K</em>, the number of coffee shops with a wireless network. On the next <em>K</em> lines, you will have 4 integers per line. The first integer <em>x</em> on each line represents the north-south street on which the coffee shop is located, where 1 �� <em>x</em> �� <em>N</em>. The second integer, <em>y</em>, on each line represents the east-west street on which the coffee shop is located, where 1 �� <em>y</em> �� <em>M</em>. The third integer, <em>R</em>, on each line represents the radius of the wireless network from this particular coffee shop. The fourth integer, <em>B</em>, on each line represents the bitrate of the wireless network from this particular coffee shop.</p>
<h3>Output</h3>
<p>The output will be two lines long. The first line of output will be the integer representing the maximum bitrate that can be obtained over all coffee shops. The second line of output will be the number of coffee shops where this maximum bitrate can be obtained.</p>
<h3>Sample Input:</h3>
<pre>3
5
3
1 3 2 5
3 1 2 7
5 1 1 5</pre>
<h3>Sample Output:</h3>
<pre>12
5</pre>
<h3>Explanation:</h3>
<p>In the figure below, notice that the five coffee shops/intersections marked with a dark circle have total bitrates of 12.<br> <img src="./24985/file/3c2gBVaz.png" alt=""></p>