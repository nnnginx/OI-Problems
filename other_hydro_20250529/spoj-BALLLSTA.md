<pre><br><span style="white-space: normal;"><p style="font-family: 'Times New Roman'; font-size: medium;">The XYZ TV channel is developing a new game show, where a contestant has to make some choices in order to get a prize. The game consists of a triangular stack of balls, each of them having an integer value, as the following example shows.</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">&nbsp;</p>
<div style="font-family: 'Times New Roman'; font-size: medium;"><img src="file://kEcesocZ.png" border="0" alt="\epsfbox{p12357.eps}" width="248" height="218" align="BOTTOM"></div>
<p style="font-family: 'Times New Roman'; font-size: medium;">The contestant must choose which balls he is going to take and his prize is the sum of the values of those balls. However, the contestant can take any given ball only if he also takes the balls directly on top of it. This may require taking additional balls using the same rule. Notice that the contestant may choose not to take any ball, in which case the prize is zero.</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">The TV show director is concerned about the maximum prize a contestant can make for a given stack. Since he is your boss and he does not know how to answer this question, he assigned this task to you.</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">&nbsp;</p>
<h2 style="font-family: 'Times New Roman';"><span style="color: #ff0000; font-size: small;">Input:</span></h2>
<p style="font-family: 'Times New Roman'; font-size: medium;">Each test case is described using several lines. The first line contains an integer&nbsp;<span><em>N</em></span>&nbsp;representing the number of rows of the stack (&nbsp;<span>1<img src="file://0sqMMcFj.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE"><em>N</em><img src="file://xL7skOWc.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE">1000</span>). The&nbsp;<span><em>i</em></span>-th of the next&nbsp;<span><em>N</em></span>&nbsp;lines contains&nbsp;<span><em>i</em></span>&nbsp;integers&nbsp;<span><em>B</em><sub>ij</sub></span>&nbsp;(&nbsp;<span>-10<sup>5</sup><img src="file://DfrposrF.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE"><em>B</em><sub>ij</sub><img src="file://cyEk8Slh.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE">10<sup>5</sup></span>&nbsp;for&nbsp;<span>1<img src="file://ljJKeA9W.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE"><em>j</em><img src="file://jfeQvNXK.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE"><em>i</em><img src="file://SC60GQpY.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE"><em>N</em></span>); the number&nbsp;<span><em>B</em><sub>ij</sub></span>&nbsp;is the value of the&nbsp;<span><em>j</em></span>-th ball in the&nbsp;<span><em>i</em></span>-th row of the stack (the first row is the topmost one, and within each row the first ball if the leftmost one).</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">The last test case is followed by a line containing one zero.</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">&nbsp;</p>
<h2 style="font-family: 'Times New Roman';"><span style="color: #ff0000; font-size: small;">Output:</span></h2>
<p style="font-family: 'Times New Roman'; font-size: medium;">For each test case output a line with an integer representing the maximum prize a contestant can make from the stack.</p>
<h2 style="font-family: 'Times New Roman';"><span style="color: #ff0000; font-size: small;">Sample input:</span></h2>
<pre>4
3
-5 3
-8 2 -8
3 9 -2 7
2
-2
1 -10
3
1
-5 3
6 -4 1
0
</pre>
<p style="font-family: 'Times New Roman'; font-size: medium;">&nbsp;</p>
<h2 style="font-family: 'Times New Roman';"><span style="color: #ff0000; font-size: small;">Sample output:</span></h2>
<pre>7
0
6</pre>
</span></pre>