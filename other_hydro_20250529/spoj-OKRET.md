<p>There is a text consisting of N characters. At each step Mirko chooses two numbers A and B and then reverses the subsequence consisting of characters between indices A and B, inclusive. Indices are 1-based.</p>
<p>Write a program that prints the final text after all operations are made.</p>
<h3>Input</h3>
<p>The first line of input contains the initial text of length N (1 ¡Ü N ¡Ü 2500000). It consists only of lowercase letters of the English alphabet.</p>
<p>The second line contains integer M (<span class="AM">1 </span>¡Ü M ¡Ü 2500), the number of steps.</p>
<p>Each of the following M lines contain two integer A and B (1 ¡Ü A ¡Ü B ¡Ü N).</p>
<h3>Output</h3>
<p>In the first and only line output the final text.</p>
<h3>Example</h3>
<pre><strong>Input:</strong> <br>lukakuka<br>3<br>1 4<br>5 8<br>1 8<br><br><strong>Output:</strong><br>kukaluka<br><strong><br><br>Input:</strong><br>kukulelebodumepcele<br>5<br>3 7<br>10 12<br>2 10<br>5 18<br>5 15<br><br><strong>Output:</strong><br>kubeeludomepcelluke<br></pre>