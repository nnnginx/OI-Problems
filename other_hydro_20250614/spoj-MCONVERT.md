<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/MCONVERT/en/">English</a></td>
<td width="50%"><a href="/problems/MCONVERT/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p><br>
</p><p>Life can be taught, but sometimes simple problems are just very well hidden among difficult ones. Once identifying those simple problems you are almost on a half way of solving them as well as making one big step towards winning the contest. Just be careful, this is NOT the simplest problem!</p>
<p>Are you ready for that challenge?</p>
<p>Your task is to write a program that transforms numbers from various numeric systems to decade one (base=10).</p>
<pre><h3 style="text-align: center;">Input</h3><br></pre>
<p>Input file consists from multiple data sets separated by one or more empty lines. First line of each set contains definition of digit ordering for some hypothetical numerical system. All ASCII printable characters (codes greater than 0x20 (space)) are allowed to appear as digits, and they are sorted according to increased decimal value (starting from zero).</p>
<p>Each line of the input data set (starting from second one) is one number coded with previously defined digits. Such numbers can have multiple decade interpretations (taking different base for hypothetical system) and your task is to find sum of all possible interpretations.</p>
<p>Explanation: If we define digit ordering as ¡°0123456789¡± possible bases are 2..10 but number ¡°6201¡± can be decoded only in systems with base 7..10. Input lines can contain white space characters on both ends which should be ignored.</p>
<pre><h3 style="text-align: center;">Output</h3></pre>
<p>You are required to output one decimal number per each number from input data sets. That number represents sum of decimal representations for all valid numeric system bases. Output data sets should be separated by one blank line.</p>
<h3 style="text-align: center;">Sample</h3>
<pre><pre>Sample input: <br>0123456789 <br> 90763 <br>1 <br> <br>.1&gt;C <br>CC. <br>&gt;.1 <br>1.... <br>Sample output: <br>90763 <br>9 <br> <br>60 <br>52 <br>353  </pre>
<br><br><strong>Note : big num - answer never has more than 1000 digits.</strong><br><br></pre>