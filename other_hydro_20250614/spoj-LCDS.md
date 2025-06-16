<p><span style="font-size: small;">GIven two sequences of integers, your task is to find the longest common subsequence where every two adjacent values differ the same.</span></p>
<p><span style="font-size: small;">For example, if the sequences are A = {1, 5, 8, 3} and B = {3, 10, 5}, then the common subsequence with adjacent values same are A<sub>L </sub>= {1, 8, 3} and B<sub>L</sub> = {3, 10, 5} since the differences in A<sub>L </sub>are 7 and -5 which is also the same in B<sub>L</sub>.<br></span></p>
<h3 style="text-align: center;"><span style="font-size: small;">Input</span></h3>
<p><span style="font-size: small;">First line of the input contains N<sub>A</sub> and N<sub>B</sub>, the sizes of the sequences A and B. Then follow two lines, the sequences A and B. (1 &lt;= N<sub>A</sub>, N<sub>B</sub> &lt;= 1000 and all values in the sequence will lie between -1e9 and 1e9).<br></span></p>
<h3 style="text-align: center;"><span style="font-size: small;">Output</span></h3>
<p><span style="font-size: small;">Print one line, the length of the LCDS as described above.<br></span></p>
<h3 style="text-align: center;"><span style="font-size: small;">Example</span></h3>
<p><span style="font-size: small;"><strong>Input:</strong><br>4 3<br>1 5 8 3<br>3 10 5<br><br><strong>Output:</strong><br>3<br><br><strong>Input:</strong><br>1 2<br>5<br>6 8<br><br><strong>Output:</strong><br>1</span></p>