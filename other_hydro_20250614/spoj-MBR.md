<p>Multiplication of natural numbers in general is a cumbersome operation. In some cases however the product can be obtained by moving the last digit to the front.<br><br>Example: 179487 * 4 = 717948<br><br>Of course this property depends on the numbersystem you use, in the above example we used the decimal representation. In base 9 we have a shorter example:<br><br>17 * 4 = 71 (base 9)<br>as (9 * 1 + 7) * 4 = 7 * 9 + 1</p>
<p><strong>Input</strong><br><br>The input for your program is a textfile. Each line consists of three numbers separated by a space: the base (&lt;=36) of the number system, the least significant digit of the first factor, and the second factor. This second factor is one digit only hence less than the base. The input file ends with the standard end-of-file marker.</p>
<p>All Numbers in input are greater than 1 and will fit in the standard "int" data type. For base &gt; 10 you can assume the digits to be 'A' ... 'Z'.</p>
<p>Note: Numbers in Input may or may not be expressed using the above digits (refer example)</p>
<p><strong>Output<br></strong><br>Your program determines for each input line the number of digits of the smallest first factor with the rotamultproperty. The output-file is also a textfile. Each line contains the answer for the corresponding input line.<br><strong></strong></p>
<p><strong>Example</strong></p>
<p><strong><br>Input</strong><br>10 7 4<br>9 7 4<br>17 14 12<br>17 E C</p>
<p><br><strong>Output:&nbsp;</strong></p>
<p>6<br>2<br>4<br>4</p>
<p>The Last two inputs are actually the same.</p>