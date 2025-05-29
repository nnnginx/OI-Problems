<p>
You are given <b>N</b> integer numbers a<sub>1</sub>, a<sub>2</sub>, ..., a<sub>N</sub>. All you need to do is to sort them in non-decreasing order.
<br><br>
The bad thing is you are only allowed to perform one action. You can pick any number in the sequence and then reverse all elements to the left and to the right of it.
<br><br>
For example, suppose you were given the sequence (7, 1, 3, 9, 8) then, depending on the picked number you'll get the following results:<br>
</p><div align="center">
<table cellspacing="5">
<tbody><tr><th>Picked number</th>
<th>Resulting sequence</th>
</tr><tr><td style="text-align: center;">7</td><td style="text-align: center;">(7, 8, 9, 3, 1)</td></tr>
<tr><td style="text-align: center;">1</td><td style="text-align: center;">(7, 1, 8, 9, 3)</td></tr>
<tr><td style="text-align: center;">3</td><td style="text-align: center;">(1, 7, 3, 8, 9)</td></tr>
<tr><td style="text-align: center;">9</td><td style="text-align: center;">(3, 1, 7, 9, 8)</td></tr>
<tr><td style="text-align: center;">8</td><td style="text-align: center;">(9, 3, 1, 7, 8)</td></tr>
</tbody></table>
</div>
<p>
In this problem you are to figure out whether the given sequence can be sorted or not, applying allowed action zero or more times.

</p><h3>Input</h3>
<p>Input will contain multiple test cases (not more than 100). Each case will start with the number of elements in the sequence N (1 ¡Ü N ¡Ü 100), followed by the N integers not exceeding 1000 by the absolute value. Input ends with the value N = 0.

</p><h3>Output</h3>
<p>For each test case write "1" if corresponding sequence can be sorted and "0" otherwise. Output must not contain spaces or line breaks.

</p><h3>Example</h3>

<pre><b>Input:</b>
5
7 1 3 9 8
2
2 1
0

<b>Output:</b>
10
</pre>