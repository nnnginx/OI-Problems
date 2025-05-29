<p>Chip and Dale have devised an encryption method to hide their (written) text messages. They first
agree secretly on two numbers that will be used as the number of rows (R) and columns (C) in a
matrix. The sender encodes an intermediate format using the following rules:
</p><ol>
<li>The text is formed with uppercase letters [A-Z] and &lt;space&gt;.
</li><li>Each text character will be represented by decimal values as follows:

<p><tt>&lt;space&gt; = 0, A = 1, B = 2, C = 3, ..., Y = 25, Z = 26</tt>
</p></li></ol>

<p>The sender enters the 5 digit binary representation of the characters¡¯ values in a spiral pattern along
the matrix as shown below. The matrix is padded out with zeroes (0) to fill the matrix completely. For
example, if the text to encode is: "ACM" and R=4 and C=4, the matrix would be filled in as follows:

</p><p><img align="center" src="./22609/file/yAqcFLgj.png">

</p><p></p><pre>A = 00001, C = 00011, M = 01101
         (one extra 0)</pre>

<p>The bits in the matrix are then concatenated together in row major order and sent to the receiver.
The example above would be encoded as: 0000110100101100

</p><h3>Input</h3>
<p>The first line of input contains a single integer N, (1 ¡Ü N ¡Ü 1000) which is the number of datasets that
follow.
</p><p>Each dataset consists of a single line of input containing R (1&lt;=R&lt;=20), a space, C (1&lt;=C&lt;=20),
a space, and a text string consisting of uppercase letters [A-Z] and &lt;space&gt;. The length of the text
string is guaranteed to be &lt;= (R*C)/5.

</p><h3>Output</h3>
<p>For each dataset, you should generate one line of output with the following values: The dataset
number as a decimal integer (start counting at one), a space, and a string of binary digits (R*C) long
describing the encoded text. The binary string represents the values used to fill in the matrix in row-
major order. You may have to fill out the matrix with zeroes (0) to complete the matrix.

</p><h3>Example</h3>

<pre><b>Input:</b>
4
4 4 ACM
5 2 HI
2 6 HI
5 5 HI HO

<b>Output:</b>
1 0000110100101100
2 0110000010
3 010000001001
4 0100001000011010110000010
</pre>