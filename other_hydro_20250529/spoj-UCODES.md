<p>Phil Oracle has a unique ability that makes him indispensable at the National Spying Agency. His colleagues can bring him any new binary code and he can tell them immediately whether the code is uniquely decodable or not. A <i>code</i> is the assignment of a unique sequence of characters (a <i>codeword</i>) to each character in an <i>alphabet</i>. A binary code is one in which the codewords contain only zeroes and ones. For example, here are two possible binary codes for the alphabet {<b>a,c,j,l,p,s,v</b>}.</p>
<img src="./24822/file/Hp7yln4H.png">
<p>The <i>encoding</i> of a string of characters from an alphabet (the <i>cleartext</i>) is the concatenation of the codewords corresponding to the characters of the cleartext, in order, from left to right. A code is <i>uniquely decodable</i> if the encoding of every possible cleartext using that code is unique. In the example above, Code 1 is uniquely decodable, but Code 2 is not. For example, the encodings of the cleartexts "<b>pascal</b>" and "<b>java</b>" are both <b>001010101010</b>. Even shorter encodings that are not uniquely decodable are <b>01</b> and <b>10</b>. 
</p><p>While the agency is very proud of Phil, he unfortunately gives only "yes" or "no" answers. Some members of the agency would prefer more tangible proof, especially in the case of codes that are not uniquely decodable. For this problem you will deal only with codes that are <i>not</i> uniquely decodable. For each of these codes you must determine the single encoding having the minimum length (measured in bits) that is ambiguous because it can result from encoding each of two or more different cleartexts. In the case of a tie, choose the encoding which comes first lexicographically.
</p><h3>Input</h3>
<p>One or more codes are to be tested. The input for each code begins with an integer m, 1&lt;=m&lt;=20, on a line by itself, where m is the number of binary codewords in the code. This is followed by m lines each containing one binary codeword string, with optional leading and trailing whitespace. No codeword will contain more than 20 bits.
</p><p>The input is terminated by the number zero on a line by itself.</p>
<h3>Output</h3>
<p>For each code, display the sequential code number (starting with 1), the length of the shortest encoding that is not uniquely decodable, and the shortest encoding itself, with ties broken as previously described. The encoding must be displayed with 20 bits on each line except the last, which may contain fewer than 20 bits. Place a blank line after the output for each code. Use the format shown in the samples below.</p>
<h3>Example</h3>
<pre><b>Input:</b>
3
0
01
10
5
0110
00
111
001100
110
5
1
001
0001
00000000000000000001
10000000000000000000
0

<b>Output:</b>
Code 1: 3 bits
010

Code 2: 9 bits
001100110

Code 3: 21 bits
10000000000000000000
1

</pre>