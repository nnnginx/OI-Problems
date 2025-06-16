<p>You are given a sequence A of <b>N</b> (<b>N</b>¡Ü250000) integers between 1 and 50000. On this sequence you have to apply <b>M</b> (<b>M</b>¡Ü10000) operations of the form: modify the i-th element in the sequence and then say how many inversions are there in the sequence. The number of inversions in a sequence is given by the number of pairs (i,j) with i &lt; j and Ai &gt; Aj.

</p><h3>Input</h3>
<p>The first line of input contains the number <b>N</b> and the next line contains the numbers that form the sequence. After that follows the number <b>M</b> and then <b>M</b> lines, each containig 2 integers X and Y, meaning that new value of the X-th element of the sequence is Y and that you should count the number of inversions in the modified sequence.

</p><h3>Output</h3>
<p>Output must contain <b>M</b> lines, the i-th line of output containg the number of inversions in the sequence after the first i operations.

</p><h3>Example</h3>

<pre><b>Input:</b>
10
2 6 6 4 7 6 3 5 9 1 
7
8 8
5 1
5 6
10 5
7 1
10 10
4 6

<b>Output:</b>
17
18
16
13
14
8
6

</pre>