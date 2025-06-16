<p><span style="font-family: arial, helvetica, sans-serif;"><br></span><span style="white-space: normal;">&nbsp;</span></p>
<p><span style="font-size: small;">Fascinated as he is by the uncanny world of electronics, our friend MKS now decides to launch his own creation --&gt; A N-Digit Carry Finder(an analogue of a N-Bit Binary Adder) which can be used to find the number of times we can have a non-zero carry while adding two numbers(A=A<sub>n</sub>A<sub>n-1</sub>...A<sub>2</sub>A<sub>1</sub> and B=B<sub>n</sub>B<sub>n-1</sub>...B<sub>2</sub>B<sub>1</sub>) having&nbsp;<strong>exactly N</strong>&nbsp;digits.</span></p>
<p><span style="font-size: small;">It consists of 'N' Full Decimal Adders. The i-th Full Adder takes as input three digits A<sub>i</sub>,B<sub>i</sub>&nbsp;and C<sub>i-1</sub>&nbsp;and outputs a digit C<sub>i</sub>(0 or 1), which is the carry generated on adding the digits A<sub>i</sub>&nbsp;and B<sub>i</sub>&nbsp;and C<sub>i-1</sub>.(C<sub>i</sub>=1 if A<sub>i</sub>+B<sub>i</sub>+C<sub>i-1&nbsp;</sub>&gt;9, otherwise 0).</span></p>
<p><span style="font-size: small;">This C<sub>i</sub>&nbsp;is now provided to the next (i+1-th) Full Adder in order to be added with the digits A<sub>i+1</sub>&nbsp;and B<sub>i+1</sub>&nbsp;and also to the accumulator which as the name suggests accumulates the sum of all C<sub>j</sub>(1&lt;=j&lt;=i).</span></p>
<p><span style="font-size: small;"><strong>Note</strong>: C<sub>0</sub>=0 always and 0&lt;=A<sub>i</sub>,B<sub>i</sub>&lt;=9.</span></p>
<p><span style="font-size: small;">For Example: Adding two numbers , A=4567 and B=734(or B=0734), the addition proceeds as shown and the accumulator gets a final value of 3.</span></p>
<p><span style="font-size: small;">In the 1st Adder, A<sub>1</sub>=7,B<sub>1</sub>=4,C<sub>0</sub>=0 and A<sub>1</sub>+B<sub>1</sub>+C<sub>0</sub>=11. Therefore Carry C<sub>1</sub>=1.</span></p>
<p><span style="font-size: small;">In the 2nd Adder, A<sub>2</sub>=6,B<sub>2</sub>=3,C<sub>1</sub>=1 and A<sub>2</sub>+B<sub>2</sub>+C<sub>1</sub>=10. Therefore Carry C<sub>2</sub>=1.</span></p>
<p><span style="font-size: small;">In the 3rd Adder, A<sub>3</sub>=5,B<sub>3</sub>=7,C<sub>2</sub>=1 and A<sub>3</sub>+B<sub>3</sub>+C<sub>2</sub>=13. Therefore Carry C<sub>3</sub>=1.</span></p>
<p><span style="font-size: small;">In the 4th Adder, A<sub>4</sub>=7,B<sub>4</sub>=0,C<sub>3</sub>=1 and A<sub>4</sub>+B<sub>4</sub>+C<sub>3</sub>=8. Therefore Carry C<sub>4</sub>=0.</span></p>
<p><span style="font-size: small;">The Value in the Accumulator=C<sub>1</sub>+C<sub>2</sub>+C<sub>3</sub>+C<sub>4</sub>=3.</span></p>
<p><span style="font-family: arial, helvetica, sans-serif;"><img title="Diagram" src="../../../content/utk1369:utk_kcarry" alt="http://www.spoj.com/content/utk1369:utk_kcarry" width="717" height="331"></span></p>
<p><span style="font-size: small;">Your Task is to find the number of ways of getting a value&nbsp;<strong>K</strong>&nbsp;in the&nbsp;<strong>accumulator</strong>&nbsp;while adding two numbers containing &nbsp;<strong>at most N</strong>&nbsp;digits each. Note that we are adding the numbers in their&nbsp;<strong>base 10</strong>&nbsp;representation. Since the total number of ways can be very large, print your answer modulo 1000000007(10^9 +7).</span></p>
<h3><span style="font-family: arial, helvetica, sans-serif;">Input</span></h3>
<p><span style="font-size: small;">The first line of input contains an integer T. Then T lines follow containing two space seperated integers N and K.</span></p>
<h3><span style="font-family: arial, helvetica, sans-serif;">Output</span></h3>
<p><span style="font-size: small;">Print the required answer modulo 1000000007(10^9 +7) in the i<sup>th</sup>&nbsp;line corresponding to the i<sup>th</sup>&nbsp;Test case .</span></p>
<p><span style="font-family: arial, helvetica, sans-serif;">&nbsp;</span></p>
<p><span style="font-size: small;"><strong><span style="font-family: arial, helvetica, sans-serif;">Constraints:</span></strong></span></p>
<p><span style="font-size: small;"><strong><span style="font-family: arial, helvetica, sans-serif;">1&lt;=T&lt;=500.</span></strong></span></p>
<p><span style="font-size: x-small;"><strong><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">1&lt;=N&lt;=1000.</span></span></strong></span></p>
<p><span style="font-size: x-small;"><strong><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">1&lt;=K&lt;=N.</span></span></strong></span></p>
<h2>Example</h2>
<h3>Sample Input</h3>
<p><span style="font-size: small;">4</span></p>
<p><span style="font-size: small;">1 1</span></p>
<p><span style="font-size: small;">2 1</span></p>
<p><span style="font-size: small;">2 2</span></p>
<p><span style="font-size: small;">3 3</span></p>
<h3>Sample Output</h3>
<p><span style="font-size: small;">45</span></p>
<p><span style="font-size: small;">4500</span></p>
<p><span style="font-size: small;">2475</span></p>
<p><span style="font-size: small;">136125</span></p>
<p><span style="font-size: small;">&nbsp;</span></p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 1142px; width: 1px; height: 1px; overflow: hidden;">Explanation</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 1142px; width: 1px; height: 1px; overflow: hidden;">Example case 1.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 1142px; width: 1px; height: 1px; overflow: hidden;">The carry appears when adding&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 1142px; width: 1px; height: 1px; overflow: hidden;">1 and 9, 2 and 9, 3 and 9 ... 9 and 9=9 cases.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 1142px; width: 1px; height: 1px; overflow: hidden;">2 and 8,3 and 8,4 and 8 ... 9 and 8=8 cases.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 1142px; width: 1px; height: 1px; overflow: hidden;">3 and 7,4 and 7,5 and 7 ... 9 and 7=7 cases.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 1142px; width: 1px; height: 1px; overflow: hidden;">.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 1142px; width: 1px; height: 1px; overflow: hidden;">.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 1142px; width: 1px; height: 1px; overflow: hidden;">.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 1142px; width: 1px; height: 1px; overflow: hidden;">9 and 1=1 case.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 1142px; width: 1px; height: 1px; overflow: hidden;">There are (9+8+7+6+5+4+3+2+1+0)=45 cases in total and in each case, the carry appears exactly once.</div>
<h2>Explanation</h2>
<p>Example case 1.</p>
<p>The carry appears when adding&nbsp;</p>
<p>1 and 9, 2 and 9, 3 and 9 ... 9 and 9=9 cases.</p>
<p>2 and 8,3 and 8,4 and 8 ... 9 and 8=8 cases.</p>
<p>3 and 7,4 and 7,5 and 7 ... 9 and 7=7 cases.</p>
<p>.</p>
<p>.</p>
<p>.</p>
<p>9 and 1=1 case.</p>
<p>There are (9+8+7+6+5+4+3+2+1+0)=45 cases in total and in each case, the carry appears exactly once.</p>
<div></div>
<p>&nbsp;</p>
<p>&nbsp;</p>