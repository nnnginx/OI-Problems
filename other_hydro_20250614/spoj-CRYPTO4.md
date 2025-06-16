<p>The Bytelandian Cryptographer has been requested by the BBFO to put forward an encryption scheme which would allow the BBFO to communicate with its foreign associates. After some intensive studies, he has decided upon the Vigenďż˝re cipher. Messages written using 26 upper case characters of the Latin alphabet: A, B, ..., Z which are interpreted as integers 0,1, ..., 25 respectively. The secret cypher for transmitting a message is known to both sides and consists of n integers k<sub>1</sub>, k<sub>2</sub>,...,k<sub>n</sub>. Using this cypher, the i-th number x<sub>i</sub> of the input message x is encrypted to the form of the i-th number of the output message y, as follows:<br>y<sub>i</sub> =(x<sub>i</sub>+k<sub>1+ ((i-1) mod n)</sub>) mod 26.
</p><p>
You are trying to find out the content of a message transmitted by the BBFO. By a lucky stroke of fortune, your spies managed to intercept the message in both its plaintext and encrypted form (x and y respectively). Unfortunately, during their dramatic escape the files they were carrying where pierced by bullets and fragments of messages x and y were inadvertently lost. Or were they? It is your task to reconstruct as much of message x as you possibly can.

</p><h3>Input</h3>
<p>The first line of input contains a single integer t&lt;=200 denoting the number of test cases. t test case descriptions follow.
</p><p>
For each test case, the first line contains one integer m which is some upper bound on the length of the cypher (1&lt;=n&lt;=m&lt;=100000). The second line of input contains the original message x, while the third line contains the encrypted message y. The messages are expressed using characters 'A'-'Z' (interpreted as integers 0-25) and '*' (denoting a single character illegible due to damage). The total length of the input file is not more than 2MB.

</p><h3>Output</h3>
<p>For each test case output a single line containing the original message x, with asterisks '*' in place of only those characters whose value cannot be determined. 

</p><h3>Example</h3>

<pre><b>Input:</b>
4
1
A*X*C
**CM*
4
*B***A
AAAAAA
6
*B***A
AAAAAA
4
*AA*******
AAAAAAAAAA

<b>Output:</b>
A*XHC
*BA*BA
*B***A
*AA**A****
</pre>
<b>Warning: large Input/Output data, be careful with certain languages.<br>The time limit is strict for this problem.</b>