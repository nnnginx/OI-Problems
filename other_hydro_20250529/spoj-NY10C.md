<p style="font-family: 'Times New Roman'; font-size: medium;">Fax machines use a form of compression based on&nbsp;run-length encoding. Run-length encoding (RLE) is a very simple form of data compression in which&nbsp;runs&nbsp;of data (that is, sequences in which the same data value occurs in many consecutive data elements) are stored as a single data value and count, rather than as the original run. This is most useful on data that contains many such runs: for example, relatively simple graphic images such as icons, text, and line drawings. It is not useful with files that don't have many runs as it could potentially double the file size (photograph, for example).</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">For this problem, you will write a program that encodes a block of data using a very simple RLE algorithm. A&nbsp;run&nbsp;is encoded using a two byte sequence. The first byte of the sequence contains the&nbsp;count, and the second contains the&nbsp;value&nbsp;to repeat. The&nbsp;count&nbsp;is encoded using an 8 bit value with the high order bit set to 1. The remaining 7 bits represent the&nbsp;count-3. This gives a maximum run count of 130 per 2 byte sequence. (This implies that the minimum run count is 3). Bytes that are not part of a&nbsp;run&nbsp;are encoded as-is with a prefix byte indicating the count of bytes in the&nbsp;non-run&nbsp;minus 1, 0 through 127, representing a range of 1 - 128 (the high order bit will always be 0 in the case of&nbsp;non-run&nbsp;data).</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">If a run contains more than 130 bytes, then it must be encoded using multiple sequences, the first of which will always be a run of 130. All&nbsp;runs&nbsp;of 3 or more&nbsp;must&nbsp;be encoded as a&nbsp;run. If a&nbsp;non-run&nbsp;contains more than 128 bytes, then multiple non-run sequences must be used. For example, a run of 262 would be encoded as two runs of 130 followed by a non-run of 2.</p>
<h2>Input</h2>
<p style="font-family: 'Times New Roman'; font-size: medium;">The first line of input contains a single integer&nbsp;<em>P</em>,&nbsp;(1<img src="file://YqPSXGhI.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE"><em>P</em><img src="file://FoVdmoM0.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE">1000), which is the number of data sets that follow. Each data set consists of multiple lines. The first line contains two (2) decimal integer values: the problem number, followed by a space, followed by the number of bytes&nbsp;<em>B</em>,&nbsp;(1<img src="file://45n0j2kc.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE"><em>B</em><img src="file://SwSIkk6L.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE">5000), to encode. The remaining line(s) contain(s) the data to be encoded. Each line of data to encode will contain 80&nbsp;hexadecimal digits&nbsp;(except the last line, which may contain less). 2&nbsp;hexadecimal digits&nbsp;are used to represent each byte. Hexadecimal digits are:&nbsp;<tt>0</tt>,&nbsp;<tt>1</tt>,&nbsp;<tt>2</tt>,&nbsp;<tt>3</tt>,&nbsp;<tt>4</tt>,&nbsp;<tt>5</tt>,&nbsp;<tt>6</tt>,<tt>7</tt>,&nbsp;<tt>8</tt>,&nbsp;<tt>9</tt>,&nbsp;<tt>A</tt>,&nbsp;<tt>B</tt>,&nbsp;<tt>C</tt>,&nbsp;<tt>D</tt>,&nbsp;<tt>E</tt>,&nbsp;<tt>F</tt>.</p>
<h2>Output</h2>
<p style="font-family: 'Times New Roman'; font-size: medium;">For each data set, there are multiple lines of output. The first line contains a decimal integer giving the data set number followed by a single space, followed by a decimal integer giving the total number of encoded bytes. The remaining lines contain the encoded data each with 80 hexadecimal digits, except the last, which may contain less.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<pre>4 
1 1 
07 
2 5 
F4A5A5A5A5 
3 44 
0000000000000000FFFFFF66665A5A5A5A5A71727374758008011011135555555555555501020399 
777777CC 
4 40 
68686868686868686868686868686868686868686868686868686868686868686868686868686868</pre>
<strong>Output:</strong>
<pre>1 2 
0007 
2 4 
00F481A5 
3 32 
850080FF016666825A0A717273747580080110111384550301020399807700CC 
4 2 
A568</pre>
</pre>