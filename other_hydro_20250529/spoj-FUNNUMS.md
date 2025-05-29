<p><span style="font-size: medium;"><span style="font-size: small;"><strong>&nbsp; &nbsp; &nbsp;&nbsp; </strong>Mr. Bean¡¯s uncle gifted him 15 English letter toys from 'a' to 'o'. As Mr. Bean is a joker, no one was  willing to play with him. So he sat on the floor and arranged these toys  in ascending order i.e. ¡°abcdefghijklmno¡±. Then he figured out the next greatest string in lexicographic order that can be formed by rearranging the toys is  ¡°</span></span><span style="font-size: medium;"><span style="font-size: small;">abcdefghijklmon</span></span><span style="font-size: medium;"><span style="font-size: small;">¡±. Now he is learning programming and wants to write a program to solve the following problem: Given a string S which can be formed by rearranging the toys, find the N-th greater string in lexicographic order. You can safely assume that such a string always exists.</span></span></p>
<p><span style="font-size: medium;"><span style="font-size: small;"><br></span></span></p>
<p><span style="font-size: small;"><strong><span style="font-size: medium;"><span style="font-size: medium;"><span style="font-size: small;">Input Specification:</span></span></span></strong></span></p>
<p><span style="font-size: medium;"><span style="font-size: medium;"><span style="font-size: small;">The  first line contains a natural number T denoting the number of test  cases. Next T lines contain the description of T test cases,  each with string S and value N.</span></span></span></p>
<p><span style="font-size: small;"><strong><span style="font-size: medium;"><span style="font-size: medium;"><span style="font-size: small;">Output Specification:</span></span></span></strong></span></p>
<p><span style="font-size: medium;"><span style="font-size: medium;"><span style="font-size: small;">For each test case print the answer in a separate line.</span></span></span></p>
<p><span style="font-size: small;"><strong><span style="font-size: medium;"><span style="font-size: medium;"><span style="font-size: small;">Input Constraints:</span></span></span></strong></span></p>
<p>&nbsp;</p>
<p><span style="font-size: medium;"><span style="font-size: medium;"><span style="font-size: small;">1&lt;=t&lt;=1000</span></span></span></p>
<p><span style="font-size: medium;"><span style="font-size: medium;"><span style="font-size: small;">2&lt;=S.length()&lt;=15</span></span></span></p>
<p><span style="font-size: medium;"><span style="font-size: medium;"><span style="font-size: small;">'a'&lt;=S[i]&lt;='a'+S.length()-1 <br></span></span></span></p>
<p><span style="font-size: medium;"><span style="font-size: medium;"><span style="font-size: small;">All letters in S are unique. <br></span></span></span></p>
<p>&nbsp;</p>
<p><span style="font-size: small;"><strong><span style="font-size: medium;"><span style="font-size: medium;"><span style="font-size: small;">Sample Input:</span></span></span></strong></span></p>
<p><span style="font-size: medium;"><span style="font-size: small;">3</span></span></p>
<p><span style="font-size: medium;"><span style="font-size: small;">abdc 2</span></span></p>
<p><span style="font-size: medium;"><span style="font-size: small;">adcb 3</span></span></p>
<p><span style="font-size: medium;"><span style="font-size: small;">badc 7<br></span></span></p>
<p><span style="font-size: small;"><strong><span style="font-size: medium;"><span style="font-size: medium;"><span style="font-size: small;">Sample Output:</span></span></span></strong></span></p>
<p><span style="font-size: small;"><span style="font-size: medium;"><span style="font-size: medium;"><span style="font-size: small;">acdb</span></span></span></span></p>
<p><span style="font-size: small;"><span style="font-size: medium;"><span style="font-size: medium;"><span style="font-size: small;">bcad</span></span></span></span></p>
<p><span style="font-size: small;"><span style="font-size: medium;"><span style="font-size: medium;"><span style="font-size: small;">cbad</span></span></span><strong><span style="font-size: medium;"><span style="font-size: medium;"><span style="font-size: small;"><br></span></span></span></strong></span></p>