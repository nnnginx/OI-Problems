<p style="margin: 1em 0px; color: #333333; line-height: 16px;"><span style="font-size: small;">ou are designing a new encryption system that works in the following way:</span></p>
<p style="margin: 1em 0px; color: #333333; line-height: 16px;"><span style="font-size: small;">For server-client communication you need a key&nbsp;<strong>k</strong>, composed of&nbsp;<strong>m</strong>&nbsp;sections, each of length&nbsp;<strong>l</strong>, and the key consists only of lowercase characters in the set {a, b, c, d, e, f}. The server has a key&nbsp;<strong>k1</strong>&nbsp;and the client has a key&nbsp;<strong>k2</strong>&nbsp;where:</span></p>
<ul style="list-style-type: none; margin: 0px; padding: 0px; color: #333333; font-family: 'lucida grande', tahoma, verdana, arial, sans-serif; font-size: 11px; line-height: 16px;">
<li><span style="font-size: small;">k1 = f(k).&nbsp;<strong>f</strong>&nbsp;is a function that receives a key and replace some random letters by ? indicating that those characters can be any lowercase letter of the set described before.</span></li>
<li><span style="font-size: small;">k2 = f(g(k)).&nbsp;<strong>g</strong>&nbsp;is a function that takes a key and produces a random permutation of its m sections. And&nbsp;<strong>f</strong>&nbsp;is the function defined above.</span></li>
</ul>
<p style="margin: 1em 0px; color: #333333; line-height: 16px;"><span style="font-size: small;">For example: let m = 3, l = 2</span></p>
<ul style="list-style-type: none; margin: 0px; padding: 0px; color: #333333; font-family: 'lucida grande', tahoma, verdana, arial, sans-serif; font-size: 11px; line-height: 16px;">
<li><span style="font-size: small;">f('abacbc') = '?ba??c'</span></li>
<li><span style="font-size: small;">g('abacbc') = 'acbcab' (each section was moved one place to the left).</span></li>
</ul>
<p style="margin: 1em 0px; color: #333333; line-height: 16px;"><span style="font-size: small;">Your task is given&nbsp;<strong>k1</strong>&nbsp;and&nbsp;<strong>k2</strong>, find key&nbsp;<strong>k</strong>. If there are several solutions, print the lexicographically smallest key. And if there is no solution at all, print "IMPOSSIBLE" (without the quotes).</span></p>
<h3><span style="font-size: small;">Input</span></h3>
<p><span style="font-size: small;"><span style="color: #333333; line-height: 16px;">The first line has a single integer&nbsp;</span><strong>T</strong><span style="color: #333333; line-height: 16px;">, which corresponds to the number of test cases.&nbsp;</span><strong>T</strong><span style="color: #333333; line-height: 16px;">&nbsp;test cases follows: the first line of the test case corresponds to the integer&nbsp;</span><strong>m</strong><span style="color: #333333; line-height: 16px;">, the second line contains the string&nbsp;</span><strong>k1</strong><span style="color: #333333; line-height: 16px;">&nbsp;and the third line contains the string&nbsp;</span><strong>k2</strong><span style="color: #333333; line-height: 16px;">.</span></span></p>
<h3><span style="font-size: small;">Output</span></h3>
<p><span style="font-size: small;"><span style="color: #333333; line-height: 16px;">For test case&nbsp;</span><strong>i</strong><span style="color: #333333; line-height: 16px;">, numbered from&nbsp;</span><strong>1</strong><span style="color: #333333; line-height: 16px;">&nbsp;to&nbsp;</span><strong>T</strong><span style="color: #333333; line-height: 16px;">, output "Case #i: ", followed by the lexicographically smallest key or "IMPOSSIBLE".</span></span></p>
<h3><span style="font-size: medium;">Example</span></h3>
<p><span style="font-size: medium;"><span style="font-size: small;">&nbsp;</span></span></p>
<p><span style="font-size: small;"><strong>Input:</strong></span></p>
<p><span style="font-size: small;">5</span></p>
<p><span style="font-size: small;">2</span></p>
<p><span style="font-size: small;">abcd</span></p>
<p><span style="font-size: small;">c?ab</span></p>
<p><span style="font-size: small;">3</span></p>
<p><span style="font-size: small;">ab?c?c</span></p>
<p><span style="font-size: small;">ac?c??</span></p>
<p><span style="font-size: small;">3</span></p>
<p><span style="font-size: small;">ab?c?c</span></p>
<p><span style="font-size: small;">aabbdd</span></p>
<p><span style="font-size: small;">2</span></p>
<p><span style="font-size: small;">aa</span></p>
<p><span style="font-size: small;">bb</span></p>
<p><span style="font-size: small;">2</span></p>
<p><span style="font-size: small;">abcd</span></p>
<p><span style="font-size: small;">cdab</span></p>
<p><span style="font-size: small;"><strong>Output:</strong></span></p>
<p><span style="font-size: small;">Case #1: abcd</span></p>
<p><span style="font-size: small;">Case #2: abacac</span></p>
<p><span style="font-size: small;">Case #3: IMPOSSIBLE</span></p>
<p><span style="font-size: small;">Case #4: IMPOSSIBLE</span></p>
<p><span style="font-size: small;">Case #5: abcd</span></p>
<p><span style="font-size: small;"><strong>Constraints :</strong></span></p>
<p><span style="font-size: small;">T &lt;= 20</span></p>
<p><span style="font-size: small;">0 &lt; |k1| &lt;= 100</span></p>
<p><span style="font-size: small;">0 &lt; m &lt;= 50</span></p>
<p><span style="font-size: small;">|k2| = |k1|</span></p>
<p><span style="font-size: small;">It is guaranteed that m is always a divisor of |k1|</span></p>
<p><span style="font-size: small;">k1 and k2 consist of {a, b, c, d, e, f, ?}</span></p>
<p>&nbsp;</p>
<pre><div id="_mcePaste" style="position: absolute; left: -10000px; top: 278px; width: 1px; height: 1px; overflow: hidden;">Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 278px; width: 1px; height: 1px; overflow: hidden;">aabbdd</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 278px; width: 1px; height: 1px; overflow: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 278px; width: 1px; height: 1px; overflow: hidden;">k1 and k2 consist of {a, b, c, d, e, f, ?}</div>
</pre>