<p>The contest just finished and you head out to show all the balloons you won to your coach who��s amazed! Contest organizers know that coders can get really excited during the five hours of contest, so they planned to take you to a flamenco performance in order to relax you a bit before the awards ceremony starts. Flamenco is indeed a traditional Spanish musical genre. The music itself is complex, and the footwork is lightning fast and must be executed with extraordinary precision. In addition the dancer may have to dance while using props such as castanets, shawls and fans.</p>
<p style="text-align: center;"><img title="castanets" src="../../../content/imuteb:castanets_2.jpg" alt="castanets" width="100" height="133"></p>
<p>The performer of this afternoon will be none other than Don Quijote de la Mancha! Unfortunately Don Quijote cannot find the scope for the castanets, nor does he remember it by heart. But he has always an encoded version of that scope with him, so that he can have a quick look at it just before the performance. As time is short, he needs your help to decode the encrypted version of the scope.<br><br>The scope can be represented as a binary string b1..bN of N digits. ��1�� stands for clap the castanet, ��0�� means leave it quiet. Now the encryption was as follows:</p>
<p style="text-align: center;"><img title="matrix" src="../../../content/imuteb:castanets_1.jpg" alt="matrix" width="152" height="155"></p>
<p>Given the original scope, the below matrix is formed from the rotated versions of the string.<br><br>Then the rows of the matrix are sorted in alphabetical order (��0�� &lt; ��1��). The last column of this matrix, read from top to bottom, is the encrypted version of the scope Don Quijote is giving you. Your task would be to find the Fth line of the matrix, which is the original version of the castanet scope.</p>
<h3>Input</h3>
<p>The input consists of no more than T (T��100) test cases. Each test case starts with two integers, which denote the number of bits N and the desired line F respectively (1��F��N��1��000). The next line contains N binary digits, the encrypted scope.</p>
<h3>Output</h3>
<p>For each test case, output the scope for the castanets.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>2<br>2 2<br>10<br>5 1<br>11100<br><br><strong>Output:</strong><br>10<br>01011<br></pre>
<h3>Note</h3>
<p>The ordered matrices for the sample test cases would be respectively</p>
<pre>01&nbsp; 01011<br>10&nbsp; 01101<br>&nbsp;&nbsp;&nbsp; 10101<br>&nbsp;&nbsp;&nbsp; 10110<br>&nbsp;&nbsp;&nbsp; 11010</pre>