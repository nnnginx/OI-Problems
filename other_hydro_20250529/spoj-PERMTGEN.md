<p>Hasan Jaddouh has invented a new algorithm for generating permutations this algorithm takes an array with length N as input and generate a permutation with length N from this array.</p>
<p>the array must satsify (1 &lt;= Ai &lt;= i) in order for the resulting array to be a permutation.</p>
<p>and here is the pseudo code of the algorithm:</p>
<pre><p><span style="font-size: x-small;"><span style="font-size: large;"><span style="color: #034c81;"><strong><span style="color: #070773;">read N<br>for i=1 to N do<br><span style="white-space: pre;">	</span>read A[i]<br>for i=1 to N do<br><span style="white-space: pre;">	</span>for j=1 to i-1 do<br><span style="white-space: pre;">		</span>if A[j] &gt;=&nbsp;A[i] do<br><span style="white-space: pre;">			</span>A[j]=A[j]+1<br>for i=1 to N do<br><span style="white-space: pre;">	</span>print A[i]</span></strong></span></span></span></p>
</pre>
<p>but unfortunately for Hasan Jaddouh, his algorithm is too slow for big arrays so he asked you to help him to find a fast way to implement&nbsp;&nbsp;his algorithm.</p>
<p>your program should read input same as the pseudo code and output the new array</p>
<h3>Input</h3>
<p>first line contains integer N (1 &lt;= N &lt;= 10<sup>5</sup>)</p>
<p>second line contains N integers separated&nbsp;by spaces each interger is between 1 and 10<sup>9</sup>&nbsp;inclusive</p>
<p><strong>note: </strong>in order for Hasan Jaddouh's algorithm to work and generate a permutation the constrain (1 &lt;= Ai &lt;= i) must be satsified but to make this problem harder this constrian is&nbsp;<strong>not </strong>guaranteed so it's also not necessary that the output is a permutation.</p>
<h3>Output</h3>
<p>Output N integers separated by spaces,&nbsp;the new array after applying Hasan Jaddouh's algorithm</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre>4</pre>
<pre>4 2 1 3</pre>
<pre><strong>Output:</strong></pre>
<pre>7 4 1 3
</pre>