<p>Andy is a really cute person and he wants to buy a koala. There are <strong>n</strong> available koalas, for each koala its beauty and cost are known. There are two accepted types of money in the world: donuts and polygons, so each koala cost can be either in donuts or polygons. Due the bad relations between The Linear States and Exponenzula no money changes between the types are allowed.<br>Help Andy to find two <strong>different</strong> koalas with the maximum total beauty so that he can buy both at the same time.</p>
<h3>Input</h3>
<p>The first line contains three integers <strong>n</strong>, <strong>d</strong> and <strong>p</strong> the number of koalas, the number of donuts and polygons Andy has.<br><br>The next <strong>n</strong> lines describe koalas. Each of these lines contain two integers b<sub>i</sub> and p<sub>i</sub> the beauty and the cost of the i-th koala, and then a letter "D" or "P", describing in which type of money is the cost of koala i: in donuts or in polygons, respectively.</p>
<h3>Output</h3>
<p>Print the maximum total beauty of exactly two koalas Andy can buy. If he can't buy two koalas, print "sad:(".</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3 7 6<br>10 8 D<br>4 3 D<br>5 6 P

<strong>Output:</strong>
9<strong><br><br>Input:</strong>
3 10 10<br>5 5 D<br>5 5 D<br>10 11 P
<strong><br>Output:</strong>
10<br></pre>
<h3>Constraints<br><br></h3>
<p>• 2 ≤ n ≤ 100000</p>
<p>• 0 ≤ d, p ≤ 100000</p>
<p>• 1 ≤ b i , p i ≤ 100000</p>