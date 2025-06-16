<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong><span style="font-family: verdana, geneva;">Tree and Palindrome | TREEPAL</span></strong></p>
<p><span style="font-family: verdana, geneva;">You are given a tree with <strong>N</strong> nodes. The tree has following properties</span></p>
<p><span style="font-family: verdana, geneva;"><br></span></p>
<ol>
<li><span style="font-family: verdana, geneva;">It is rooted at node 1</span></li>
<p><span style="font-family: verdana, geneva;"><br></span></p>
<li><span style="font-family: verdana, geneva;">Node 1 situated in level 0. The children of node 1 is situated in level 1 ,&nbsp; the children of the level 1 nodes is situated in level 2&nbsp; , the children of the level 2 nodes is situated in level 3 and so on ��.... .</span></li>
<p><span style="font-family: verdana, geneva;"><br></span></p>
<li><span style="font-family: verdana, geneva;">Every node is marked by an alphabet. The nodes of the same level are marked by the same alphabet.</span></li>
<p><span style="font-family: verdana, geneva;"><br></span></p>
<li><span style="font-family: verdana, geneva;">Level zero nodes are marked by 'a' , level 1 nodes are marked by 'b' , level 2 nodes are marked by 'c'</span></li>
<p><span style="font-family: verdana, geneva;">��... level 25 nodes are marked by 'z', level 26 nodes are marked again by 'a', level 27 nodes are marked by 'b' and so on �� (the leveling is rotational).</span></p>
<p><span style="font-family: verdana, geneva;"><br></span></p>
<li><span style="font-family: verdana, geneva;">If we take all the alphabets of the nodes serially which are in the path from node a to node b (including a, b) and concatenate them, then we find a string. The name of the string is <strong>Bokkor</strong> string of pair (a, b).</span></li>
<p><span style="font-family: verdana, geneva;"><br></span></p>
</ol>
<p><span style="font-family: verdana, geneva;">You will be given a pair of distinct nodes. You don't know in advance which pair will be given. The probability of choosing every pair is same. Now your job is to calculate the probability that the <strong>Bokkor</strong> string of the given pair is a palindrome in <strong>p/q </strong>format (where p and q are co-prime).<br></span></p>
<ol>
<p><span style="font-family: verdana, geneva;"><br></span></p>
<p align="center"><img src="file://oImDtEub.png" alt="Tree Structure"></p>
<p align="center"><span style="font-family: verdana, geneva;"><br> Figure: Tree Structure</span></p>
<p align="center"><span style="font-family: verdana, geneva;"><br></span></p>
</ol>
<p><span style="font-family: verdana, geneva;">Here the pair (2, 3) forms the Bokkor string ��bab�� which is a palindrome.</span><br><span style="font-family: verdana, geneva;">And the pair (4, 5) forms the Bokkor string ��cbabc�� which is also a palindrome.</span><br><span style="font-family: verdana, geneva;">There are no other palindromic Bokkor pairs.</span><br><span style="font-family: verdana, geneva;"><img src="file://g6uIWlhd.png" alt="Equation" width="687" height="52"></span></p>
<p><span style="font-family: verdana, geneva;">&nbsp;&nbsp;</span></p>
<p><strong>&nbsp;</strong></p>
<!--[if gte msEquation 12]><m:oMathPara><m:oMath><m:f><m:fPr><span     style="font-size:14.0pt;mso-ansi-font-size:14.0pt;mso-bidi-font-size:14.0pt;     font-family:"Cambria Math","serif";mso-ascii-font-family:"Cambria Math";     mso-hansi-font-family:"Cambria Math";font-style:italic;mso-bidi-font-style:     normal" mce_style="font-size:14.0pt;mso-ansi-font-size:14.0pt;mso-bidi-font-size:14.0pt;     font-family:"Cambria Math","serif";mso-ascii-font-family:"Cambria Math";     mso-hansi-font-family:"Cambria Math";font-style:italic;mso-bidi-font-style:     normal"><m:ctrlPr></m:ctrlPr></span></m:fPr><m:num><i style="mso-bidi-font-style:     normal" mce_style="mso-bidi-font-style:     normal"><span style="font-size:14.0pt;line-height:115%;font-family:"Cambria Math","serif";     mso-fareast-font-family:Calibri;mso-fareast-theme-font:minor-latin;     mso-bidi-font-family:Vrinda;mso-bidi-theme-font:minor-bidi;mso-ansi-language:     EN-US;mso-fareast-language:EN-US;mso-bidi-language:AR-SA" mce_style="font-size:14.0pt;line-height:115%;font-family:"Cambria Math","serif";     mso-fareast-font-family:Calibri;mso-fareast-theme-font:minor-latin;     mso-bidi-font-family:Vrinda;mso-bidi-theme-font:minor-bidi;mso-ansi-language:     EN-US;mso-fareast-language:EN-US;mso-bidi-language:AR-SA"><m:r>Total</m:r><m:r> </m:r><m:r>numbers</m:r><m:r> </m:r><m:r>of</m:r><m:r> </m:r><m:r>Bokkor</m:r><m:r> </m:r><m:r>pairs</m:r></span></i></m:num><m:den><i style="mso-bidi-font-style:     normal" mce_style="mso-bidi-font-style:     normal"><span style="font-size:14.0pt;line-height:115%;font-family:"Cambria Math","serif";     mso-fareast-font-family:Calibri;mso-fareast-theme-font:minor-latin;     mso-bidi-font-family:Vrinda;mso-bidi-theme-font:minor-bidi;mso-ansi-language:     EN-US;mso-fareast-language:EN-US;mso-bidi-language:AR-SA" mce_style="font-size:14.0pt;line-height:115%;font-family:"Cambria Math","serif";     mso-fareast-font-family:Calibri;mso-fareast-theme-font:minor-latin;     mso-bidi-font-family:Vrinda;mso-bidi-theme-font:minor-bidi;mso-ansi-language:     EN-US;mso-fareast-language:EN-US;mso-bidi-language:AR-SA"><m:r>Total</m:r><m:r> </m:r><m:r>numbers</m:r><m:r> </m:r><m:r>of</m:r><m:r> </m:r><m:r>possible</m:r><m:r> </m:r><m:r>pairs</m:r><m:r> </m:r></span></i></m:den></m:f></m:oMath></m:oMathPara><![endif]--><!--[if !msEquation]--><!--[endif]-->
<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 666px; width: 1px; height: 1px; overflow: hidden;">&nbsp;Total numbers of Bokkor pairs &nbsp; &nbsp; &nbsp; 2 &nbsp; &nbsp; &nbsp;1 &nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 666px; width: 1px; height: 1px; overflow: hidden;">&nbsp;----------------------------- &nbsp;= &nbsp; -- &nbsp;= &nbsp; - &nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 666px; width: 1px; height: 1px; overflow: hidden;">&nbsp;Total numbers of Bokkor pairs &nbsp; &nbsp; &nbsp;10 &nbsp; &nbsp; &nbsp;5 &nbsp;</div>
<p><strong>Input</strong><strong>&nbsp;</strong></p>
<p><span style="font-family: verdana, geneva;">There will be multiple testcases. The first line of each test case starts with a number </span><strong>N</strong><span style="font-family: verdana, geneva;"> </span><strong>(3&lt;=N&lt;=10<sup>5</sup>) </strong><span style="font-family: verdana, geneva;">which denotes the number of nodes in the tree. Next </span><strong>N-1</strong><span style="font-family: verdana, geneva;"> line of the test-case each consists of a pair of integers </span><strong>u, v (1&lt;= u, v&lt;=N and u! = v) </strong><span style="font-family: verdana, geneva;">which denotes there is an edge between u and v. It is guaranteed that the input is legal (no multiple edges and it forms a valid tree)</span><br><span style="font-family: verdana, geneva; font-weight: bold;">&nbsp;</span></p>
<p><span style="font-family: verdana, geneva; font-weight: bold;">Output</span><br><span style="font-family: verdana, geneva;">For each test case output is just a single line </span><strong>��p/q�� </strong><span style="font-family: verdana, geneva;">(without the quotes) as described above. It is guaranteed that p&gt;=1.</span></p>
<p>&nbsp;</p>
<table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="319" valign="top">
<p><strong><span style="font-family: verdana, geneva;">Sample Input</span></strong></p>
</td>
<td width="319" valign="top">
<p><strong><span style="font-family: verdana, geneva;">Output for Sample Input</span></strong></p>
</td>
</tr>
<tr>
<td width="319" valign="top">
<p><span style="font-size: small;">5</span></p>
<p><span style="font-size: small;">1 2</span></p>
<p><span style="font-size: small;">1 3</span></p>
<p><span style="font-size: small;">2 4</span></p>
<p><span style="font-size: small;">3 5</span></p>
<p><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;">6</span></p>
<p><span style="font-size: small;">1 2</span></p>
<p><span style="font-size: small;">1 3</span></p>
<p><span style="font-size: small;">3 4</span></p>
<p><span style="font-size: small;">3 5</span></p>
<p><span style="font-size: small;">2 6</span></p>
</td>
<td width="319" valign="top">
<p><span style="font-size: small;">1/5</span></p>
<p><span style="font-size: small;">4/15</span></p>
</td>
</tr>
</tbody>
</table>
<p><strong> N.B. Dataset is huge, use faster IO</strong></p>
<p><strong>Problem Setter: Syed Shahriar Manjur</strong></p>
<p><strong>Special Thanks: Abdullah Al Maruf , Ahmad Faiyaz</strong></p>