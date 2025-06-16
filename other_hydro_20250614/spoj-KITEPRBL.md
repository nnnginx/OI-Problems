<p>Bob, owner of kite factory decided to make some good money.</p>
<p>He has bought new machine to produce kites, but this machine doesn't have any software in it ! He was very sad, oh, so very sad. Every kite is produced from big square sheet of paper.</p>
<p>He didn't want to spend next big sum of money hiring programmists, so he decided to ask you for help.</p>
<p>He wants his machine to :</p>
<p>-cut exactly as much color paper as needed to cover kite and then cover it immidiately</p>
<p>-make N very little small holes in the kite ( through which he can put colorful bows and other shiny things )</p>
<p>-at the end he wants his machine to sort convex shape kites and non-convex shapes kites ( he thinks that convex shape kites should be transported to "Biedronka" - shop for poor people, so he doesn't want to mix them with really expensive ones )</p>
<h3>Input</h3>
<p>In first line there is number T, number of test cases.</p>
<p>In first line of each test case there is number X(X&lt;200), number of verticles of the each kite.</p>
<p>Then X pairs of number, xi and yi, coords of each verticle.</p>
<p>Left-bottomst corner of paper have (0,0) coords.</p>
<p>In next line number N(N&lt;20000), number of holes to make in the kite.</p>
<p>Then N number, xi and yi, coords of each hole to make in the kite.</p>
<p>Obviously, hole cannot be made on the perimeter of kite.</p>
<p>We can assume that no three points are colinear, also there is no point duplicate. Bob always would give you verticles of kite in clockwise order.</p>
<h3>Output</h3>
<p>For each test case print area ( 10^-3 precision ) of paper which was used to produce each kite, holes which were made successfully, and digit 1 if kite is convex shape, otherwise digit 0. Separate each test case with new line</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>1<br>6<br>0 0<br>5 0<br>4 2<br>5 4<br>0 4<br>1 2<br>3<br>1 1<br>1 2<br>5 2<br><br><strong>Output:</strong><br>32.000 1 0<br><br>Explaination: 32.000 area of paper to cover the kite. Only 1st hole can be made successfully (2nd is on parimeter, 3rd is out the kite)<br>Kite has non-convex shape<br></pre>