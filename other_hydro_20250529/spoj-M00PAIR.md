<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td style="text-align: center;" width="50%"><a href="/problems/M00PAIR/en/">English</a></td>
<td style="text-align: center;" width="50%"><a href="/problems/M00PAIR/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>A sequence consisting of one digit,  the number 1  is  initially written into a computer. At each successive  time  step,  the  computer  simultaneously tranforms each digit 0 into  the  sequence 1 0 and each digit 1  into the sequence 0 1.</p>
<p>So, after  the  first time step,  the sequence 0 1  is obtained; after the second, the sequence 1 0 0 1, after the third, the sequence 0 1 1 0 1 0 0 1 and so on.</p>
<p>How many pairs of consequitive zeroes will appear in the sequence after n steps?</p>
<h3 style="text-align: center;">Input</h3>
<p>Clarification for this Problem: The Range of inputs is from 1 to 999 in some order and in particular not in ascending order</p>
<h3 style="text-align: center;">Output</h3>
<p style="text-align: center;">For each input n print the number of consequitive zeroes pairs that will appear in the sequence after n steps.</p>
<h3 style="text-align: center;">Sample</h3>
<pre>Sample Input <br>1<br>2 <br>3 <br>4<br>5 <br>Sample output <br>0<br>1 <br>1<br>3<br>5<br> </pre>
<p><strong>Notice : Long output - 1.45MB </strong> - there are a lot of input/output so it is easy to TLE if you dont optimize in/out if you use Java ... </p>