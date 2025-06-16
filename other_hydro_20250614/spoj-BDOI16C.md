<p style="margin-bottom: 0.14in;" align="CENTER"><span style="font-size: medium;"><strong>Counting Permutations</strong></span></p>
<p style="margin-bottom: 0.14in;" align="JUSTIFY"><span style="font-size: small;"><a name="_GoBack"></a>In a planet far away from Earth, there is a beautiful country named Magicland. The children of this country play a lot of interesting games with numbers. One of the most popular games is called Inversion. In this game, you will be given numbers from 1 to N. They are given in a certain order. You need to calculate all the inversions in the given permutation of the numbers. S/he who can say it first correctly wins the game. An inversion occurs when there exists a pair of indices i and j such that i &lt; j and given number at i-th position is greater than the number at j-th position.</span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0.14in;" align="JUSTIFY"><span style="font-size: small;">For example, let us consider a permutation of numbers 1 to 5: 5, 1, 4, 2, 3. This permutation has the following inversions: (5, 1), (5, 4), (5, 2), (5, 3), (4, 2), (4, 3). Therefore, the number of inversion will be 6. The first person to tell this number correctly will win this game.</span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0.14in;" align="JUSTIFY"><span style="font-size: small;">For this problem, we want to know how many permutations of the numbers 1, 2, .., N will have at least K inversions.</span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0.14in;" align="JUSTIFY"><span style="font-size: small;">A permutation X is different from another permutation Y if there exists some <em>i (1&lt;=i&lt;=N)</em> for which the number in i-th position is different in these two permutations.</span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0.14in;" align="JUSTIFY"><span style="font-size: small;"><strong>Input</strong></span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0.14in;" align="JUSTIFY"><span style="font-size: small;">The first line of input file contains the number of test cases, <strong>T (1&lt;=T&lt;=50)</strong>. Then <strong>T</strong> cases follow:</span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0.14in;" align="JUSTIFY"><span style="font-size: small;">Each case consists of one line which contains two integers: <strong>N</strong> and <strong>K.</strong></span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0.14in;" align="JUSTIFY"><span style="font-size: small;"><strong>Constraint</strong></span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0.14in;" align="JUSTIFY"><span style="font-size: small;">For Easy version, <strong>1&lt;=N&lt;=200 </strong>and<strong> 0&lt;=K&lt;=300.</strong></span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0.14in;" align="JUSTIFY"><span style="font-size: small;">For Hard version, <strong>1&lt;=N&lt;=2000 </strong>and<strong> 0&lt;=K&lt;=3000.</strong></span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0.14in;" align="JUSTIFY"><span style="font-size: small;"><strong>Output</strong></span></p>
<p><span style="font-size: small;"> </span></p>
<p style="margin-bottom: 0.14in;" align="JUSTIFY"><span style="font-size: small;">For each case, print ¡°<strong>Case x: y</strong>¡± in a separate line, where <strong>x </strong>is the case number and <strong>y</strong> is the number of permutations with at least <strong>K</strong> inversions. As the number can be very large, print <strong>y</strong> <strong>modulo 10,007</strong>.</span></p>
<table style="width: 638px;" border="0" cellspacing="0" cellpadding="7">
<colgroup><col width="304"> <col width="304"> </colgroup> 
<tbody>
<tr valign="TOP">
<td style="border: 1px solid #00000a; padding-top: 0in; padding-bottom: 0in; padding-left: 0.08in; padding-right: 0.08in" width="304">
<p align="JUSTIFY"><span style="font-size: small;">Sample 			Input</span></p>
</td>
<td style="border: 1px solid #00000a; padding-top: 0in; padding-bottom: 0in; padding-left: 0.08in; padding-right: 0.08in" width="304">
<p align="JUSTIFY"><span style="font-size: small;">Sample 			Output</span></p>
</td>
</tr>
<tr valign="TOP">
<td style="border: 1px solid #00000a; padding-top: 0in; padding-bottom: 0in; padding-left: 0.08in; padding-right: 0.08in" width="304">
<p style="margin-bottom: 0in" align="JUSTIFY"><span style="font-family: Courier New,serif;"><span style="font-size: x-small;">3</span></span></p>
<p style="margin-bottom: 0in" align="JUSTIFY"><span style="font-family: Courier New,serif;"><span style="font-size: x-small;">3 			1</span></span></p>
<p style="margin-bottom: 0in" align="JUSTIFY"><span style="font-family: Courier New,serif;"><span style="font-size: x-small;">2 			1</span></span></p>
<p align="JUSTIFY"><span style="font-family: Courier New,serif;"><span style="font-size: x-small;">3 2</span></span></p>
</td>
<td style="border: 1px solid #00000a; padding-top: 0in; padding-bottom: 0in; padding-left: 0.08in; padding-right: 0.08in" width="304">
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-size: small;">Case 			1: 5</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-size: small;">Case 			2: 1</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-size: small;">Case 			3: 3</span></p>
<p align="JUSTIFY"><span style="font-size: small;"><br></span></p>
</td>
</tr>
</tbody>
</table>
<p style="margin-bottom: 0.14in" align="JUSTIFY"><span style="font-size: medium;"><strong>Problem Setter: Anindya Das</strong></span><br><br></p>