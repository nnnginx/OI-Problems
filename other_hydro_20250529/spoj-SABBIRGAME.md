<p>Sabbir is a little boy. he loves &nbsp;to play. One day his friend taskin suggested a new interesting game. there are n levels in the game. one should pass all the levels with a positive life-point. in some level one can increase his life-point by defeating the villain of the game or lose some life-point when one can't defeat the villain. Sabbir knows the points he is going to lose or increase in each level. determine the mnimum life-point sabbir should have initially ( at the starting of the game ) to pass all the levels with a positive life point.</p>
<h3>Input</h3>
<p>input consists of at most 100 test cases.</p>
<p>first line consists of a single integer T ( 1 &lt;= T &lt;= 100) number of test cases</p>
<p>each test case is consists of two lines. first line consists of an integer n ( 1 &lt;= n &lt;= 1000 )</p>
<p>second line consists of n space separated&nbsp;integer &nbsp;a<sub>1 </sub>, a<sub>2 </sub>..... a<sub>n-1 </sub>, a<sub>n </sub>( -10<sup>7</sup><sup>&nbsp;</sup>&lt;= a<sub>i &nbsp;</sub>&lt;= 10<sup>7</sup><sup>&nbsp;</sup>)<sub>&nbsp;</sub></p>
<h3>Output</h3>
<p>for each test case print an integer in one line , the minimum life-point sabbir will need initially.</p>
<h3>Example</h3>
<pre><strong><span style="font-size: medium;">Input:</span></strong>
3<br>3<br>5 -8 3<br>4<br>1 2 -3 5<br>3<br>1 0 3</pre>
<pre><strong><span style="font-size: medium;">Output:</span></strong></pre>
<pre>4<br>1<br>0</pre>
<pre><span style="font-size: small;">explanation:</span></pre>
<pre><span style="font-size: small;">first case, if sabbir have 4 life-points at first. sabbir will have 9 points after playing 1st level, he will have 1 point after playing 2nd level, he will have 4 points after playing 3rd level... his points never  becomes less than 1 (remains positive) . if he start with a lower point ( less than 4) initially, he will die at the 2nd level and can't pass all the levels. so, 4 is the minimum ans</span>.</pre>