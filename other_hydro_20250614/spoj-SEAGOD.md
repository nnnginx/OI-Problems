<p>Jesse is a biologist and he was studying some aspects of life when he discovered that certain<br>species of sea animals tried to tell him some things about God. Those animals were using a certain<br>language to speak with him. They wrote down in binary code (black and white) in the shell they have.<br>As Jesse was the only one that this message was intended to be delivered, they encrypted the message<br>in such way that there is a rule to decrypt every bit in the spherical-shaped shell looking at 3 other bit:<br>the left, itself and the right in this order. So first they write the cyphered message and the rule to<br>decrypt it in lexicographical order, so the rule space in the shell containing the bit to decrypt ¡°101¡± will<br>be rule's bit 5. To turn the cryptography more elaborated there is also the number of rounds that this<br>must be done to the entire message. Jesse wants to hire you to write a program for him to decrypt the<br>text and live in harmony forever and ever with the animals he loves and find out who is and what this<br>God wants to do.</p>
<h3>Input</h3>
<p>The input has several test cases. The first line of a test case contains the message length L (0 &lt; L ¡Ü<br>10000). The next line contains the message M, of length L bits. In the next line, your program should<br>read the 8-bits rule R. In another line, the number of rounds 0 ¡Ü N ¡Ü 10000. Your program must read<br>until the end of file.</p>
<h3>Output</h3>
<p>For each test case your program must write the message M after applying the rule R for N rounds.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5<br>10111<br>10101010<br>1<br>10<br>1011010101<br>11100010<br>2

<strong>Output:</strong>
10000<br>1011010101</pre>