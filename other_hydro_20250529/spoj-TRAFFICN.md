<p>The city traffic network consists of n nodes numbered from 1 to n and m one-way roads connecting pairs of nodes. In order to reduce the length of the shortest path between two different critical nodes s and t, a list of k two-way roads are proposed as candidates to be constructed.  Your task is to write a program to choose one two-way road from the proposed list in order to minimize the resulting shortest path between s and t.</p>
<h3>Input</h3>
<p>The input file consists of several data sets. The first line of the input file contains the number of data sets which is a positive integer and is not bigger than 20. The following lines describe the data sets.</p>
<p>For each data set, the first line contains five positive integers n (n ¡Ü 10 000), m (m ¡Ü 100 000), k (k &lt; 300), s (1 ¡Ü s ¡Ü n), t (1 ¡Ü t ¡Ü n) separated by space. The ith line of the following m lines contains three integers di, ci, li separated by space, representing the length li ( 0&lt; li ¡Ü 1000) of the ith one-way road connecting node di to ci. The jth line of the next k lines contains three positive integers uj, vj and qj (qj ¡Ü 1000) separated by space, representing the jth proposed two-way road of length qj connecting node uj to vj.</p>
<h3>Output</h3>
<p>For each data set, write on one line the smallest possible length of the shortest path after building the chosen one two-way road from the proposed list. In case, there does not exist a path from s to t, write -1.</p>
<h3>Example</h3>
<pre><strong>Sample Input</strong>
1
4 5 3 1 4
1 2 13
2 3 19
3 1 25
3 4 17
4 1 18
1 3 23
2 3 5
2 4 25	

<strong>Sample Output</strong>
35
</pre>