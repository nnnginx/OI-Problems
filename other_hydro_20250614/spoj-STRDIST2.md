<p style="text-align: justify;">Prof.XYZ is an expert in sequence analysis. One such problem he works on is   bar-coding DNA sequences. The problem at hand is, given two DNA   sequences, find a way to compute their similarity efficiently. Formally a   DNA sequence is a string (S) of length N where each character is from a   set  of symbols derived from a vocabulary б╞. We define the  m-perturbed set of a string S to be&nbsp; жд(S,m)  which contains the set of  all strings S' obtained by changing atmost m  characters of S with  m&lt;=N. In other words, жд(S,m) is the set of all strings S' such that  the hamming distance between S and S' (defined by H(S,S')) is atmost m.&nbsp;</p>
<p style="text-align: justify;">&nbsp;</p>
<p style="text-align: justify;">Prof.XYZ defines an order (m1,m2) similarity between two   N-length strings S1 and S2 to be the number of strings in the   intersection of жд(S1,m1) and жд(S2,m2). It is easy to see that the number   of strings in this intersection only depends on the hamming distance   between S1 and S2 (rather than the entire original strings S1 and S2). In other  words |жд(S1,m1) б╔ жд(S2,m2)| is only a function of N, the hamming distance  H(S1,S2), m1, m2 and the alphabet size |б╞|. Your objective is to write a program that counts the size of  this  intersection given&nbsp; N, m1, m2, H(S1,S2) and&nbsp;  |б╞|. Since the  answer can be very large, output the answer modulo 1000000007.</p>
<h3 style="text-align: justify;">Input</h3>
<p>The first line of the input contains the number of test cases T (atmost 50). Each testcase consists of 5 integers in order</p>
<p>&nbsp;(1) N : The length of each of the two strings. 1&lt;=N&lt;=1000</p>
<p>&nbsp;(2) m1 : The allowed number of changes in the first string. 0&lt;=m1 &lt;= min(100,N/2)</p>
<p>&nbsp;(3) m2 : The allowed number of changes in the second string. 0&lt;=m2 &lt;=min(100,N/2)</p>
<p>&nbsp;(4) H(S1,S2): The hamming distance between the two strings. 0&lt;=H &lt;=min(100,N/2)</p>
<p>&nbsp;(5) |б╞| : The size of the vocabulary. 2&lt;=|б╞|&lt;=1000000</p>
<h3 style="text-align: justify;">Output</h3>
<p>For each test-case output the required number of strings in the intersection modulo 1000000007 in a seperate line.</p>
<p>&nbsp;</p>
<h3 style="text-align: justify;">Example</h3>
<pre style="text-align: justify;"><strong>Input:</strong><br>3<br>6 1 2 2 2<br>10 2 2 3 5<br>20 3 4 5 7<br><br><br><strong>Output:</strong><br>3<strong><strong><br></strong></strong>24<strong><strong><br></strong></strong>1925<strong><strong><br><br>Explanation (for the first test case)</strong></strong></pre>
<p style="text-align: justify;">The length of each string is 6. We are allowed to perturb atmost one element from the first string and atmost two elements from the second. Since their hamming distance needs to be two, let S1=000000 be the first string and S2=000011 be the second. The set жд(S1,1) is&nbsp; {000000,000001,000010,000100,001000,010000,100000}. Without enumerating жд(S2,2), we can see that the only set of strings in жд(S1,1) that can be obtained by perturbing atmost two elements in S2 are {000000,000001,000010}. Thus |жд(S1,m1) б╔ жд(S2,m2)| =3.</p>
<pre>&nbsp;</pre>