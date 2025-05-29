<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/GLOVE/en/">English</a></td>
<td width="50%"><a href="/problems/GLOVE/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p> </p>
<p>In the dark basement of chemistry professor Acidrain¡¯s house there are two drawers with gloves ¡ª one with left hand and other with right hand gloves. In each of them there are gloves of n different colours. Professor knows how many gloves of each colour there are in each drawer (the number of gloves of the same colour may differ in both drawers). He is also sure that it is possible to find a pair of gloves of the same colour.</p>
<p>Professor¡¯s experiment may be successful only if he uses gloves of the same colour (it does not matter which one), so before every experiment he goes to the basement and takes gloves from the drawers hoping that there will be at least one pair of the same colour. It is so dark in the basement that there is no possibility to recognize colour of any glove without going out of the basement. Professor hates going to the basement more than once (in case there was no pair of gloves of the same colour), as well as  bringing unnecessarily large amounts of gloves to the laboratory.</p>
<p>&nbsp;</p>
<h3>Task</h3>
<p>Write a program that:</p>
<ul>
<li> reads the number of colours and the number of gloves in each colour in each drawer from the standard input, </li>
<li> calculates the smallest total number of gloves which must be taken to be sure that among them it is possible to find at least one pair of gloves of the same colour (it is necessary to specify the exact number of gloves to be taken from each drawer), </li>
<li> writes the result to the standard output. </li>
</ul>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line of the standard input contains one positive integer n (1 ¡Ü n ¡Ü 20 ) describing the number of distinct colours. The colours are numbered from 1 to n. The second line of input contains n non-negative integers 0 ¡Ü a1,a2, . . .an ¡Ü 10^8, where ai corresponds to the number of gloves of colour number i in the drawer with left hand gloves. Finally, the third line of input contains n non-negative integers 0 ¡Ü b1, b2, . . . , bn ¡Ü 10^8, where bi corresponds to the number of gloves of colour number i in the drawer with right hand gloves.</p>
<h3>Output</h3>
<p>The first line of the standard output should contain a single integer ¡ª the number of gloves which must be taken from the drawer with left hand gloves. The second line of output should contain a single integer ¡ª the number of gloves which must be taken from the drawer with right hand gloves. The sum of these two numbers should be as small as possible. If there are several correct results, your program should output any of them.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4
0 7 1 6
1 5 0 6


<strong>Output:</strong>
2
8


</pre>