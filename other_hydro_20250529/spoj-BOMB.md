<p>You want to destroy a bridge with bombs. The lower-left corner of the bridge is at (0,0) and the upper-right corner is at (w,l). There are already b bombs exploded, the i-th bomb created a hole of radius ri centering at (xi,yi). You want to throw exactly one more bomb so that the bridge is split into two connected parts(though the two parts can share a finite number of points), so that no one can go through the bridge from y = 0 to y = l. Your task is to find the minimal radius of the last bomb to split the bridge, assuming that the last bomb can explode precisely at the position you want (possibly at non-integer coordinates). Note that you are only allowed to use bombs with integer radius. That is, even if a bomb with radius 1.01 is sufficient, you have to use a bomb with radius 2, since you only have bombs with integer radius.</p>
<h3>Input</h3>
<p>The first line contains t (1¡Üt¡Ü10), the number of test cases followed. Each test case begins with three integers w,l,b(1¡Üw,1¡Ü100, 0¡Üb¡Ü10). Each of the following b lines contains three integers integers xi,yi,ri(0¡Üx¡Üw, 0¡Üy¡Ül, 0£¼r¡Ü100). The bridge is guaranteed to be connected before the last bomb.</p>
<h3>Output</h3>
<p>For each test case, print the minimal radius of the last bomb.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p>3<br>100 100 2<br>15 50 20<br>90 50 30<br>100 100 1<br>50 50 40<br>100 100 1<br>10 50 10</p><p>&nbsp;</p>
<strong>Output:</strong>
13<br>50<br>40<br></pre>