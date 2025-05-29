<p>Chip and Dale have devised an encryption method to hide their (written) text messages. They first
agree secretly on two numbers that will be used as the number of rows (R) and columns (C) in a
matrix. The sender encodes an intermediate format using the following rules:
</p><ol>
<li>The text is formed with uppercase letters [A-Z] and <space>.
</space></li><li>Each text character will be represented by decimal values as follows:

<p><tt><space> = 0, A = 1, B = 2, C = 3, ..., Y = 25, Z = 26</space></tt>
</p></li></ol>

<p>The sender enters the 5 digit binary representation of the characters¡¯ values in a spiral pattern along
the matrix as shown below. The matrix is padded out with zeroes (0) to fill the matrix completely. For
example, if the text to encode is: "ACM" and R=4 and C=4, the matrix would be filled in as follows:

</p><p><img align="center" src="./22610/file/spcCIaIv.png">

</p><p></p><pre>A = 00001, C = 00011, M = 01101
         (one extra 0)</pre>

<p>The bits in the matrix are then concatenated together in row major order and sent to the receiver.
The example above would be encoded as: 0000110100101100

</p><h3>Input</h3>
<p>The first line of input contains a single integer N, (1 ¡Ü N ¡Ü 1000) which is the number of datasets that
follow.
</p><p>Each dataset consists of a single line of input containing R (1&lt;=R&lt;=20), a space, C (1&lt;=C&lt;=20),
a space, and a string of binary digits that represents the contents of the matrix (R * C binary digits).
The binary digits are in row major order.

</p><h3>Output</h3>
<p>For each dataset, you should generate one line of output with the following values: The dataset
number as a decimal integer (start counting at one), a space, and the decoded text message. You
should throw away any trailing spaces and/or partial characters found while decoding.

</p><h3>Example</h3>

<pre><b>Input:</b>
4
4 4 0000110100101100
5 2 0110000010
2 6 010000001001
5 5 0100001000011010110000010

<b>Output:</b>
1 ACM
2 HI
3 HI
4 HI HO
</pre>