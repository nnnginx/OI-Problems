<p>Arithmatic and geometric Progressions are 2 of the well known progressions in maths.</p>
<p>Arithmatic progression(AP) is a set in which the difference between 2   numbers in constant. for eg, 1,3,5,7,9 .... In this series the   difference between 2 numbers is 2.</p>
<p>Geometric progression(GP) is a set in which the ratio of 2   consecutive numbers is same. for eg, 1,2,4,8,16.... In this the ratio of   the numbers is 2.</p>
<p>.....</p>
<p>What if there is a series in which we multiply a(n) by 'r' to get a(n+1) and then add 'd' to a(n+1) to get a(n+2)...</p>
<p>For eg .. lets say d=1 and r=2 and a(1) = 1..</p>
<p>series would be 1,2,4,5,10,11,22,23,46,47,94,95,190 ......</p>
<p>We add d to a(1) and then multiply a(2) with r and so on ....</p>
<p>&nbsp;</p>
<p>Your task is, given 'a' , 'd'&nbsp; &amp;&nbsp; 'r' to find the a(n) term .</p>
<p>sicne the numbers can be very large , you are required to print the numbers modulo 'mod' - mod will be supplied int the test case.</p>
<h3>Input</h3>
<p>first line of input will have number 't' indicating the number of test cases.</p>
<p>each of the test cases will have 2 lines</p>
<p>firts line will have 3 numbers 'a' ,'d'&nbsp; and&nbsp;&nbsp; 'r'</p>
<p>2nd line will have 2 numbers 'n' &amp; 'mod'</p>
<p>a- first term of the AGS</p>
<p>d-the difference element</p>
<p>r - the ratio element</p>
<p>n- nth term required to be found</p>
<p>mod- need to print the result modulo mod</p>
<h3>Output</h3>
<p>For each test case print "a(n)%mod" in a separate line.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>1 1 2<br>13 7<br>2 2 2<br>10 8<br><br>&nbsp;<strong>Output:</strong><br><br>1<br>6 <br><br><br>Description - for the first test case the series is 1,2,4,5,10,11,22,23,46,47,94,95,190..<br>13th term is 190 and 190%7 = 1<br><br><strong>Note </strong>- the value of a , d , r , n &amp; mod will be less than 10^8 and more than 0.<br>for every series 2nd term will be a+d and third term will be (a+d)*r .. and so on ..</pre>