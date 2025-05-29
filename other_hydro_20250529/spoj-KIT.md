<pre><span style="white-space: normal;"><p>Krypt in Time</p>
<p>&nbsp;</p>
<p>In a land far away people can travel back in time in person or send messages to them in the past. Sending messages that can change ones future is forbidden. The messages that are sent are intercepted by the time police.&nbsp; Jim wants to send a message to himself in the past to prevent his death. He decides to encrypt using a "number-pad".&nbsp; All the numbers in number-pad are between 0 and 25. The message he wants to send can be encrypted if each character in the string is encoded by a number from the pad provided each number from the number- pad is only used once. The encryption is done by shifting each letter in the message by k positions, where k is determined by the number-pad. Shift occurs between the alphabets "a" and "z". If a letter in the message is shifted past "z" then it starts back at "a" and continues to shift.</p>
<p>For example:&nbsp; If the number-pad contains 2, the message abc is transformed to cde and xyz to zab.</p>
<p>&nbsp;</p>
<p>Input Format</p>
<p>The first line will contain the size of the number-pad N, followed by a sequence of numbers for the pad. The remaining input consists of a series of words to be encrypted using the number-pad. You may assume that the maximum size of the pad (N) is 100 numbers, all numbers in the pad are between 0 and 25, and that all input will be lowercase letters. The end of input is indicated by -1.</p>
<p>&nbsp;</p>
<p>Output Format</p>
<p>For each word to be encrypted, output a line containing the encrypted word.</p>
<p>&nbsp;</p>
<p>Example</p>
<p>Input 1:<br>
10<br>
1 2 3 4 5 4 3 2 1 0<br>
aa aaa<br>
zzzzz<br>-1</p><p>
Output 1:<br>
bc<br>
def<br>
dcbaz</p></span></pre>