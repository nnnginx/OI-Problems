<p><span style="font-size: x-large;"><strong>Perfect Superstring</strong></span></p>
<p><img src="../../../content/tjandra:C_cover.png" alt=""></p>
<p>Satria is a smart person, after he understand the system of binary digits he immediately write a new challenge! The challenge is, give him a binary string S he will tell you a binary string B which is not substring of S. Because Satria is smart, he will always tell buinary string B with minimum length. But everything has a limit, even Satria's intelligence, his brain will be tired if he check subtring of S of length more than N. So he can't tell the binary string B if the binary string S containing all the possible B of length ¡ÜN, in orther word S is superstring of all possible binary string B of length ¡ÜN, lets call S "Perfect Superstring" of order N if it meet this consition.</p>
<p>Gunawan know this challenge and Satria's intelligence limit want to make a binary string S which is perfect superstring of order N. Then he write down all possible binary string B, and concatenate them. For example if he want to make perfect superstring of order 2, he will write: {0,1,00,01,10,11} and concatenate to 0100011011 and submit it. Unfortunately Satria is so smart so his limit will be high. So the Gunawan method to generating perfect superstring of order high is inefficient, but Gunawan never give up, he insist to write his perfect superstring using his method.</p>
<p>After Gunawan writing K digits of his binary string, Tjandra who is curious about Gunawan's serous face ask him why he is so serious.</p>
<p><span style="text-decoration: underline;">Tjandra said</span>: "What are you doing?"<br><span style="text-decoration: underline;">Gunawan replied</span>: "I want to solve Satria's challange"<br><span style="text-decoration: underline;">Tjandra replied</span>: "Sound interesting, can you explain the challenge?"<br>(Gunawan explaining Satria's challenge)<br><span style="text-decoration: underline;">Tjandra said</span>: "wow, that's interesting, how do you solve this challenge?"<br>(Gunawan explaining his method)<br><span style="text-decoration: underline;">Tjandra said</span>: "That's inefficient, it's enough to concatenate possible binary string B of length N, forget about binary string that has length less than N because all of them will eventually be substring of binary string which has large length, for example if you want to make perfect superstring of order 2 your string will be 0100011011, but it's enough to just concatenate {00,01,10,11} and become 00011011, it's shorter and it's perfect superstring of length 2!"<br><span style="text-decoration: underline;">Gunawan replied</span>: "wow it's shorter! I never think about that, is that the minimum possible length"<br><span style="text-decoration: underline;">Tjandra replied</span>: "No, there are the shorter one, for example in binary string 000110011 the substring 11 appear 2 times, so we can delete one digit of '1's and i't still meet the perfect superstring of order 2"<br><span style="text-decoration: underline;">Gunawan replied</span>: "You're right, I don't like wasting my energy, I want the perfect superstring of order N with minimum possible length!"<br><span style="text-decoration: underline;">Tjandra replied</span>: "Unfortunately no simple method for generating the minimum posible length of perfect superstring, but I know someone who can generate it for you with modern computer"<br>(Tjandra pulled his old phone from his pocket, getting ready to call you for help)<br><span style="text-decoration: underline;">Gunawan said</span>: "Wait, I already write K binary digits, I don't want to delete them and start from the beginning"<br><span style="text-decoration: underline;">Tjandra replied</span>: "What -_- Ok, I'll consider that"</p>
<p>Now Tjandra call you using his old phone for help, because he know you're skilled at string processing. Can you help them?</p>
<p><span style="font-size: large;"><strong>Input</strong></span></p>
<p>The first line there is an integer N denoting the order of perfect superstring on Satria's challenge.<br>On the second line there are one integer K and one string X, K denoting the length of binary string that is already writen by Gunawan, and X is that binary string itself.</p>
<p><strong><span style="font-size: large;">Output</span></strong></p>
<p>The the first line you should output minimum possible length of {perfect superstring of order N starting with X of length K}, let's call this number L.<br>On the second line you should output a binary string of length L starting with K and it is perfect superstring of order N.</p>
<p><strong><span style="font-size: large;">Constraint</span></strong></p>
<p>1 ¡Ü N ¡Ü 20</p>
<p>0 ¡Ü K ¡Ü N</p>
<p>String X will have length K, in order word |X|=K. <span style="text-decoration: underline;">It can be empty string if K=0</span>.</p>
<p><strong><span style="font-size: large;">Sample 1</span></strong></p>
<p><span style="text-decoration: underline;">Input</span></p>
<pre>1<br>1 0</pre>
<p><span style="text-decoration: underline;">Output</span></p>
<pre>2<br>01</pre>
<p><strong><span style="font-size: large;">Sample 2</span></strong></p>
<p><span style="text-decoration: underline;">Input</span></p>
<pre>1<br>1 1</pre>
<p><span style="text-decoration: underline;">Output</span></p>
<pre>2<br>10</pre>
<p><strong><span style="font-size: large;">Sample 3</span></strong></p>
<p><span style="text-decoration: underline;">Input</span></p>
<pre>2<br>2 01</pre>
<p><span style="text-decoration: underline;">Output</span></p>
<pre>5<br>01100</pre>
<p><strong><span style="font-size: large;">Sample 4</span></strong></p>
<p><span style="text-decoration: underline;">Input</span></p>
<pre>3<br>3 110</pre>
<p><span style="text-decoration: underline;">Output</span></p>
<pre>10<br>1101000111</pre>
<p><strong><span style="font-size: large;">Sample 5</span></strong></p>
<p><span style="text-decoration: underline;">Input</span></p>
<pre>3<br>3 110</pre>
<p><span style="text-decoration: underline;">Output</span></p>
<pre>10<br>1100010111</pre>
<p><strong><span style="font-size: large;">Sample 4 (and 5) Explanation</span></strong></p>
<p>In sample 4, string 1101000111 starting with string 110: [110]1000111, so Gunawan doesn't need to erase his already written number from the begining.</p>
<p>It also meet the perfect supertring of order 3 because all binary string of length ¡Ü3 is substring of that string.</p>
<p>Here is the proof:</p>
<p>0: 11<strong><span style="text-decoration: underline;">0</span></strong>1000111<br>1: <strong><span style="text-decoration: underline;">1</span></strong>101000111<br>00: 1101<strong><span style="text-decoration: underline;">00</span></strong>0111<br>01: 11<strong><span style="text-decoration: underline;">01</span></strong>000111<br>10: 1<strong><span style="text-decoration: underline;">10</span></strong>1000111<br>11: <strong><span style="text-decoration: underline;">11</span></strong>01000111<br>000: 1101<strong><span style="text-decoration: underline;">000</span></strong>111<br>001: 11010<strong><span style="text-decoration: underline;">001</span></strong>11<br>010: 11<strong><span style="text-decoration: underline;">010</span></strong>00111<br>011: 110100<strong><span style="text-decoration: underline;">011</span></strong>1<br>100: 110<strong><span style="text-decoration: underline;">100</span></strong>0111<br>101: 1<strong><span style="text-decoration: underline;">101</span></strong>000111<br>110: <strong><span style="text-decoration: underline;">110</span></strong>1000111<br>111: 1101000<strong><span style="text-decoration: underline;">111</span></strong></p>
<p>Note that there can be multiple solution, the string 1100010111 as shown on sample 5 is another minimal length perfect superstring of of order 3 starting with 110.</p>