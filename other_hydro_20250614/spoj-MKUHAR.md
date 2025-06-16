<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/MKUHAR/en/">English</a></td>
<td width="50%"><a href="/problems/MKUHAR/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>Lisa works as a waitress  in a restaurant. Tonight  is her birthday so Lisa asked  the chef  to prepare his special meal for her friends. The chef's meal  is made of N  ingredients. To prepare one serving of the meal he needs a certain amount of each ingredient.</p>
<p>There  are  some  ingredients  already  available  in  the  kitchen  and Lisa will  buy  the  rest  at  the  grocery store. The store has all the necessary ingredients, each coming in smaller and larger packages. Lisa has M dollars and wants to spend them so that the chef can make the most servings of his meal.</p>
<pre><br></pre>
<h1>Input</h1>
<p>The first line contains two integers N and M, 1 ≤ N ≤ 100, 1 ≤ M ≤ 100 000. Each  of  the  following N  lines  contains  6  positive  integers, information  about  one  ingredient. These specify, in order:</p>
<p style="padding-left: 30px;">•  X, 10 ≤ X ≤ 100, the amount of the ingredient needed in one serving;</p>
<p style="padding-left: 30px;">•  Y, 1 ≤ Y ≤ 100, the amount of the ingredient already available in the kitchen;</p>
<p style="padding-left: 30px;">•  SM, 1 ≤ SM &lt; 100, the size of the smaller package at the store;</p>
<p style="padding-left: 30px;">•  PM, 10 ≤ PM &lt; 100, the price of the smaller package;</p>
<p style="padding-left: 30px;">•  SV, SM &lt; SV ≤ 100, the size of the larger package; and</p>
<p style="padding-left: 30px;">•  PV, PM &lt; PV ≤ 100, the price of the larger package.</p>
<pre style="padding-left: 30px;"></pre>
<h1>Output</h1>
<p>Output the largest number of servings the chef can make if Lisa spends her money wisely.</p>
<h1>Sample</h1>
<pre>input <br> <br>2 100 <br>10 8 10 10 13 11 <br>12 20 6 10 17 24 <br> <br>output <br> <br>5<br><br>input <br> <br>3 65 <br>10 5 7 10 13 14 <br>10 5 8 11 14 15 <br>10 5 9 12 15 16 <br> <br>output <br> <br>2<br></pre>
<p>In  the  first  example,  for  99  dollars  Lisa  will  buy  three  smaller and  one  larger  package  of  the  first ingredient, as well as one smaller and two larger packages of the second ingredient (3x10 + 1x11 + 1x10 + 2x24 = 99).</p>
<p>The chef will then have 51 units (8 + 3x10 + 1x13) of the first ingredient and 60 units (20 + 1x6 + 2x17) of the second ingredient, enough for 5 servings.</p>
<pre> </pre>
<p> </p>