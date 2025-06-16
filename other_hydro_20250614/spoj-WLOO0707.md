<p>After a day trip with his friend Dick, Harry noticed a strange pattern of tiny holes in the door of his SUV. The local American Tire store sells fiberglass patching material only in square sheets. What is the smallest patch that Harry needs to fix his door?
<br><br>
Assume that the holes are points on the integer lattice in the plane. Your job is to find the area of the smallest square that will cover all the holes.

</p><h3>Input</h3>
<p>The first line of input contains a single integer T expressed in decimal with no leading zeroes, denoting the number of test cases to follow. The subsequent lines of input describe the test cases.
<br><br>
Each test case begins with a single line, containing a single integer n expressed in decimal with no leading zeroes, the number of points to follow; each of the following n lines contains two integers x and y, both expressed in decimal with no leading zeroes, giving the coordinates of one of your points.
<br><br>
You are guaranteed that T &lt;= 30 and that no data set contains more than 30 points. All points in each data set will be no more than 500 units away from (0,0).

</p><h3>Output</h3>
<p>Print, on a single line with two decimal places of precision, the area of the smallest square containing all of your points. An answer will be accepted if it lies within 0.01 of the correct answer.

</p><h3>Example</h3>

<pre><b>Input:</b>
2
4
-1 -1
1 -1
1 1
-1 1
4
10 1
10 -1
-10 1
-10 -1

<b>Output:</b>
4.00
242.00
</pre>