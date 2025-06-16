<p>Ada the Ladybug got a new homework today. She was attending algebra class and teacher was lecturing about various utilizations of matrix multiplication. He wanted to teach his students about the power of matrix, so he gave them following homework:</p>
<p>Students were given a matrix followed be multiple queries. The query of first kind is adding a number to each element of a rectangular region of their matrix. In the query of second kind, a matrix is given and students are asked, whether it is the second power of actual matrix.</p>
<p>Can you help Ada to solve her homework?</p>
<p><span style="font-size: 1.17em;">Input</span></p>
<p>The first line contains two integers <strong>1 ¡Ü N ¡Ü 150 </strong>, the size of square matrix and <strong> 1 ¡Ü Q ¡Ü 200 </strong>, the number of queries.</p>
<p>Each of the next <strong>N</strong> lines contains <strong>N</strong> integers <strong>0 ¡Ü     A<sub>x,y</sub> ¡Ü 100</strong>, the element on <strong>x<sup>th</sup>,y<sup>th</sup></strong> coordinate of matrix.</p>
<p>Then <strong>Q</strong> queries follows:</p>
<p>The query of first kind is <strong>1</strong> followed five integers  <strong>0 ¡Ü x, y     ¡Ü X, Y &lt; N</strong>, specifing the part, to which the number will be added, and number <strong>0 ¡Ü V ¡Ü 100</strong>, the value which will be added.</p>
<p>The query of second kind is <strong>2</strong> followed by <strong>N</strong> lines containing <strong>N</strong> integers, which are supposed to be the second power of actual matrix.</p>
<h3>Output</h3>
<p>For each query of second kind, print either <strong>yes</strong>, if given matrix is second power of actual state of matrix or <strong>no</strong> in the other case.</p>
<h3>Example Input</h3>
<pre>2 5
1 2
2 1
2
5 4
4 5
2
4 5
5 4
1 0 1 1 1 1
2
7 9
6 10
2
5 4
4 5
</pre>
<h3>Example Output</h3>
<pre>yes
no
yes
no
</pre>
<h3>Example Input 2</h3>
<pre>5 10
66 60 69 84 23
69 81 94 91 66
24 38 35 65 28
31 27 91 57 11
4 5 40 0 71
1 3 0 4 0 79
2
21301 13825 21173 20277 9967
27887 17060 26586 24464 15252
14519 7743 13488 11454 6743
18490 13839 18940 20861 8268
12676 7260 10437 10027 8400
1 1 0 4 2 100
1 2 4 3 4 37
1 2 2 2 2 1
1 0 2 0 3 4
2
46237 38485 46414 21029 16080
96987 88160 100456 49140 37497
73915 66266 75834 36015 28535
79761 74224 83550 45701 31771
60176 56760 62709 34759 25280
2
46237 38485 46414 21029 16080
96987 88160 100456 49140 37497
73915 66266 75835 36015 28535
79761 74224 83551 45701 31771
60176 56760 62709 34759 25280
2
46237 38486 46414 21028 16080
96987 88160 100456 49140 37497
73915 66265 75835 36016 28535
79761 74224 83551 45701 31771
60176 56760 62709 34759 25280
2
46237 38485 46414 21029 16080
96987 88160 100456 49140 37497
73915 66266 75835 36015 28535
79761 74224 83551 45701 31771
60176 56760 62709 34759 25280
</pre>
<h3>Example Output 2</h3>
<pre>no
no
yes
no
yes
</pre>