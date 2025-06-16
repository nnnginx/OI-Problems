<p>Alice and Bob need to send secret messages to each other and are discussing ways to encode their
messages:</p>
<blockquote>
<p>
	<u>Alice:</u> ¡°Let¡¯s just use a very simple code: We¡¯ll assign ¡®A¡¯ the code word 1, ¡®B¡¯ will be 2,
	and so on down to ¡®Z¡¯ being assigned 26.¡±<br></p>
<p>
	<u>Bob:</u> ¡°That¡¯s a stupid code, Alice. Suppose I send you the word ¡®BEAN¡¯ encoded as 25114.
	You could decode that in many different ways!¡±<br>
</p>
<p>
	<u>Alice:</u> ¡°Sure you could, but what words would you get? Other than ¡®BEAN¡¯, you¡¯d get
	¡®BEAAD¡¯, ¡®YAAD¡¯, ¡®YAN¡¯, ¡®YKD¡¯ and ¡®BEKD¡¯. I think you would be able to figure out the
	correct decoding. And why would you send me the word ¡®BEAN¡¯ anyway?¡±<br>
</p>
<p>
	<u>Bob:</u> ¡°OK, maybe that¡¯s a bad example, but I bet you that if you got a string of length 5000
	there would be tons of different decodings and with that many you would find at least two
	different ones that would make sense.¡±<br>
</p>
<p>
	<u>Alice:</u> ¡°How many different decodings?¡±<br>
</p>
<p>
	<u>Bob:</u> ¡°Jillions!¡±
</p>
</blockquote>
<p>
For some reason, Alice is still unconvinced by Bob¡¯s argument, so she requires a program that will
determine how many decodings there can be for a given string using her code.</p>
<h3>Input</h3>
<p>Input will consist of multiple input sets. Each set will consist of a single line of at most 5000 digits representing a
valid encryption (for example, no line will begin with a 0). There will be no spaces between the digits.
An input line of ¡®0¡¯ will terminate the input and should not be processed.</p>
<h3>Output</h3>
<p>For each input set, output the number of possible decodings for the input string. All answers will be
within the range of a 64 bit signed integer.</p>
<h3>Example</h3>

<pre><b>Input:</b>

25114
1111111111
3333333333
0

<b>Output:</b>

6
89
1
</pre>