<p> The ancient mathematician and philosopher Pythagoras believed that reality is
mathematical in nature. Present-day biologists study properties of biosequences. A
biosequence is a sequence of M integers, which<br>
• contains each of the numbers 0,1,…,M-1,<br>
• starts with 0 and ends with M-1, and<br>
• has no two elements E,E+1 in adjacent positions in this order.<br>
A subsequence consisting of adjacent elements of a biosequence is called a segment..<br><br>
A segment of a biosequence is called a framed interval if it includes all integers whose
values are between the value of the first element, which must be the smallest element in the
segment, and the last element, which must be the largest and different from the first. A
framed interval is called an empodio if it does not contain any shorter framed intervals.<br><br>
As an example, consider the biosequence (0,3,5,4,6,2,1,7). The whole biosequence is a
framed interval. However, it contains another framed interval (3,5,4,6) and therefore it is
not an empodio. The framed interval (3,5,4,6) does not contain a shorter framed interval, so
it is an empodio. Furthermore, it is the only empodio in that biosequence.<br><br>
You are to write a program that, given a biosequence, finds all empodia (plural for empodio)
in that biosequence.
</p>

<h3>Input</h3>
<p>
t - the number of test cases [t &lt;= 20], then t test cses follows. 
The first line of each test case contains a single integer M: the number
of integers in the input biosequence. The following M lines contain the integers of the
biosequence in the order of the sequence. Each of these M lines contains a single integer.
In one test case, 1000000 &lt;= M &lt;= 1100000. In all other test cases, 1 &lt;= M &lt;= 60000.
Additionally, in 50% of the test cases, M &lt;= 2600.
</p>

<h3>Output</h3>
<p>The first line for each test case is to contain one integer H:
the number of empodia in the input biosequence. The following H lines describe all
empodia of the input biosequence in the order of appearance of the starting point in the
biosequence. Each of these lines is to contain two integers A and B (in that order) separated
by a space, where the Ath element of the input biosequence is the first element of the
empodio and the Bth element of the input biosequence is the last element of the empodio.
<br>  
</p>

<h3>Example</h3>
<pre><b>Input:</b>
1
8 
0 
3 
5 
4 
6 
2 
1 
7
</pre>
<pre><b>Output:</b>
1
2 5
</pre>