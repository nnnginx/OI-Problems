<p>Thursday 25/7/2013, a friend of mine (<a href="../../../users/hossameldeen/" target="_blank">Goodname</a>) posted in our facebook group (Virtual Contests) a link of <a href="http://community.topcoder.com/tc?module=MemberProfile&amp;cr=8416646" target="_blank">Kawigi</a>'s topcoder profile.</p>
<p>He was amazed by Kawigi's quote as he tested it in <a href="http://ideone.com/MSrP0c" target="_blank">Ideone</a> to find it printing "C++Sucks". We all were amazed by this quote.</p>
<p>But in a few minutes some other friend of mine (<a href="../../../users/mc_mosa/" target="_blank">Mosa</a>) commented on the post with this <a href="http://ideone.com/AUPTQx" target="_blank">Ideone</a>.  Wow! he got it, but the fact that he is kind of greedy, he didn't want  to tell us the secret. Now we want to think like Mosa to be able to  solve this problem.</p>
<p>Given a string your task is to find the values of m[0] and m[1] so that when we run this code we get the given string.</p>
<h3 style="text-align: center;">Code</h3>
<p>#include &lt;stdio.h&gt;</p>
<p>int primes [] = {2,3,5,7,11};<br><br>double m[2] = {8242465576917890.0 ,494};<br><br>int main() {<br>&nbsp; m[1]--?m[0]/=primes[((int)m[1]+1)%5],main():printf((char*)m);<br>}</p>
<p><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">// this code prints the string "123".<br></span></span></p>
<h3 style="text-align: center;">Input</h3>
<p>The first line of the input file contains an integer T (T &lt;= 50) which is the number of test cases to follow.</p>
<p>Each test case will be on a single line consisting of at most 6 alphanumeric characters (A-Za-z0-9).</p>
<h3 style="text-align: center;">Output</h3>
<p>For each test case, print the values of m[0] and m[1], separated by a space.</p>
<p>It's guaranteed that the solution will always exist. If there're multiple solutions, print any.</p>
<h3 style="text-align: center;">Example</h3>
<pre><strong>Input:</strong>
4<br>123<br>abdou<br>mcMosa<br>kimo3<br><br><strong>Output:</strong>
8242465576917890.0 494<br>6966198460426549.0 487<br>4484456159639948.0 483<br>21357815651012032.0 488</pre>
<h4 style="text-align: left;">Special Thanks:</h4>
<p>-<a href="../../../users/cyclops/" target="_blank">Mitch Schwartz</a> for discovering issues with the problem.</p>
<p>-<a href="../../../users/mc_mosa/" target="_blank">Mosa Osama</a> for writing the special judge of the problem, and I have to say Mosa's not greedy. ;)</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 456px; width: 1px; height: 1px; overflow: hidden;">&nbsp;</div>