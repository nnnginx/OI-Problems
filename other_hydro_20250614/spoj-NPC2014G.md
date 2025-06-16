<p>Joke is a student at a famous University called Tenth November Institute of Technology. As a student, Joke is very active at university organizations. The organizations that he join includes science, social, even politic. Not only becoming an activist, Joke is also one of the leaders of those organizations. Since he is so busy, he doesn't have much time to study. So now he wants to focus on his academic.</p>
<p>On the last year of his study, Joke can't decide the topic for his thesis. Joke asks Joan, his friend for help. Since Joan likes mathematics, Joan gives Joke a topic about positive integers. After thinking for a few days, Joan found the topic that he thinks is suitable for Joke. Joke is very happy to hear that. When they meet each other, Joke buys Joan some delicious cake.</p>
<p>After reaching his house, Joke reads the topic that was given by Joan. He is shocked and disappointed. Joke thinks he can't do that topic. He really wants to ask for other people's help, but then he realizes that he doesn't have any more money to buy a cake. As a good friend of Joke, you told him that you will help him for free. Joke is very happy and now he told you the topic of his thesis. Given N numbers, you must find the total number of parity value of each pair of the numbers. Parity value is defined as the following:</p>
<ol>
<li>At first, the parity value (P) of both numbers is zero.</li>
<li>Make a parameter of parity (S) with the value 2.</li>
<li> 
<ul>
<li>If both numbers are divisible by S, add P by zero.</li>
<li>If both numbers are not divisible by S, add P with S/2, then subtract both numbers with S/2.</li>
<li>If only one of them is divisible by S, add P with zero, and subtract the one that is not divisible by S with S/2.</li>
</ul>
</li>
<li>Multiply S by 2.</li>
<li>Repeat step 3 and 4 until both numbers is zero.</li>
</ol>
<p>Your task is to find the sum of parity number of each pair in a list of N number.</p>
<h3>Input</h3>
<p>First line contains a number N.</p>
<p>The next N lines contain A<span style="vertical-align: sub;">i</span>, which represents the ith number. A<span style="vertical-align: sub;">i</span>&nbsp;will fit in signed 32 bit integer.</p>
<h3>Output</h3>
<p>Output the sum of parity value of the numbers. Since the number can be so big, output the result modulo 1000000007.</p>
<h3>Sample Input</h3>
<pre>3
7
7
7</pre>
<h3>Sample Output</h3>
<pre>21</pre>
<div style="border: 1px solid #FC0; background-color: #ffc; padding: 5px; margin-bottom: 10px;">
<h3>Constraint</h3>
<p>1 ¡Ü N ¡Ü 1000000</p>
<p><span style="font-size: 10.3999996185303px;">A</span><span style="font-size: 10.3999996185303px; vertical-align: sub;">i</span><span style="font-size: 10.3999996185303px;">&nbsp;will fit in signed 32 bit integer</span></p>
</div>