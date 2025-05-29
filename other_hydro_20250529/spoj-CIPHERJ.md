<h1 style="text-align: center;"><span style="font-size: small;"><span style="font-weight: normal;"><br></span></span></h1>
<p>Bob and Alice started to use a brand-new encoding scheme. Surprisingly it is not a Public Key Cryptosystem, but their encoding and decoding is based on secret keys. They chose the secret key at their last meeting in Philadelphia on February 16th, 1996. They chose as a secret key a sequence of&nbsp;<em>n</em>&nbsp;distinct integers,&nbsp;<img src="./21832/file/lY6Un1EC.png" alt="tex2html_wrap_inline27" width="72" height="17" align="MIDDLE">&nbsp;, greater than zero and less or equal to&nbsp;<em>n</em>. The encoding is based on the following principle. The message is written down below the key, so that characters in the message and numbers in the key are correspondingly aligned. Character in the message at the position&nbsp;<em>i</em>&nbsp;is written in the encoded message at the position&nbsp;<img src="./21832/file/7fITZndZ.png" alt="tex2html_wrap_inline33" width="13" height="17" align="MIDDLE">&nbsp;, where&nbsp;<img src="./21832/file/PhmgJeBh.png" alt="tex2html_wrap_inline33" width="13" height="17" align="MIDDLE">&nbsp;is the corresponding number in the key. And then the encoded message is encoded in the same way. This process is repeated&nbsp;<em>k</em>&nbsp;times. After&nbsp;<em>k</em>th encoding they exchange their message.</p>
<p>The length of the message is always less or equal than&nbsp;<em>n</em>. If the message is shorter than&nbsp;<em>n</em>, then spaces are added to the end of the message to get the message with the length&nbsp;<em>n</em>.</p>
<p>&nbsp;</p>
<p>Help Alice and Bob and write program which reads the key and then a sequence of pairs consisting of&nbsp;<em>k</em>&nbsp;and message to be encoded&nbsp;<em>k</em>&nbsp;times and produces a list of encoded messages.</p>
<p><strong><span style="font-size: small;">Input</span></strong></p>
<p>The input file consists of several blocks. Each block has a number&nbsp;<img src="./21832/file/Bgdwo8UB.png" alt="tex2html_wrap_inline51" width="90" height="25" align="MIDDLE">&nbsp;in the first line. The next line contains a sequence of&nbsp;<em>n</em>&nbsp;numbers pairwise distinct and each greater than zero and less or equal than&nbsp;<em>n</em>. Next lines contain integer number&nbsp;<em>k</em>&nbsp;and one message of ascii characters separated by one space. The lines are ended with eol, this eol does not belong to the message. The block ends with the separate line with the number 0. After the last block there is in separate line the number 0.</p>
<p><strong><span style="font-size: small;">Output</span></strong>&nbsp;</p>
<p>Output is divided into blocks corresponding to the input blocks. Each block contains the encoded input messages in the same order as in input file. Each encoded message in the output file has the lenght&nbsp;<em>n</em>. After each block there is one empty line.</p>
<p><strong><span style="font-size: small;">Sample Input</span></strong></p>
<pre>10
4 5 3 7 2 8 1 6 10 9
1 Hello Bob
1995 CERC
0
0
</pre>
<p><strong><span style="font-size: small;">Sample Output</span></strong></p>
<pre>BolHeol  b
C RCE     </pre>