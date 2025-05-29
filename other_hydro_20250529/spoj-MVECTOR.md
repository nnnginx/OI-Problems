<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/MVECTOR/en/">English</a></td>
<td width="50%"><a href="/problems/MVECTOR/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>We can represent a 2D vector as a pair (X,Y).  The sum of two or more vectors is a vector whose coordinates  are the sums of the corresponding coordinates of all the vectors in  the sum.  e.g. (1,2)+(3,4)+(5,6) = (1+3+5,2+4+6) = (9,12)  Weight of a vector (x,y) is defined as x*x+y*y.  You are given N vectors on a plain.</p>
<p>Your task is to write a program that will determine a subset of  those vectors so the weight of the sum of all vectors in that subset is  maximal.</p>
<p>Note: Use 64-bit integers (int64 in pascal or long long in c)</p>
<h3>Input</h3>
<p>In the first line of the input file is an integer N, 1 ¡Ü N ¡Ü 30,000,  the number of vectors.</p>
<p>The following N lines contain descriptions for each of the vectors.  A description is made of two integers X and Y, separated by a single  blank, -30,000 ¡Ü X,Y ¡Ü 30,000.</p>
<p>None of the given vectors will be (0,0)</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>In the first and only line of the output file you have to write the  weight of the maximum sum.</p>
<h3>Sample</h3>
<pre>suma.in <br> <br>5 <br>5 -8 <br>-4 2 <br>4 -2 <br>2 1 <br>-6 4 <br> <br>suma.out <br> <br>202 <br><br>suma.in <br> <br>4 <br>1 4 <br>-1 -1 <br>1 -1 <br>-1 4 <br> <br>suma.out <br> <br>64<br><br>suma.in <br> <br>9 <br>0 1 <br>6 8 <br>0 -1 <br>0 6 <br>-1 1 <br>-1 2 <br>5 -4 <br>1 0 <br>6 -5 <br> <br>suma.out <br> <br>360 <br></pre>
<p> </p>