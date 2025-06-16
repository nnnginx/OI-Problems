<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/MKTHNUM/en/">English</a></td> 
<td width="50%"><a href="/problems/MKTHNUM/vn/">Vietnamese</a></td> 
</tr></tbody></table>

<p></p><p>
You are working for Macrohard company in data structures department. After 
failing your previous task about key insertion you were asked to write a
new data structure that would be able to return quickly k-th order statistics
in the array segment.
</p><p>
That is, given an array a[1 ... n] of different integer numbers, your 
program must answer a series of questions Q(i, j, k) in the form: "What would
be the k-th number in a[i ... j] segment, if this segment was sorted?"
</p><p>
For example, consider the array a = (1, 5, 2, 6, 3, 7, 4). Let the question
be Q(2, 5, 3). The segment a[2 ... 5] is (5, 2, 6, 3). If we sort this 
segment, we get (2, 3, 5, 6), the third number is 5, and therefore the
answer to the question is 5. 
</p><p>
</p><h3>Input</h3>
<p></p><p>
The first line of the input contains n ¡ª the size of the array, and m ¡ª 
the number of questions to answer (1 ¡Ü n ¡Ü 100000, 1 ¡Ü m ¡Ü 5000).
</p><p>
The second line contains n different integer numbers not exceeding 10^9 
by their absolute values ¡ª the array for which the answers should be given.
</p><p>
The following m lines contain question descriptions, each description consists
of three numbers: i, j, and k (1 ¡Ü i ¡Ü j ¡Ü n, 1 ¡Ü k ¡Ü j - i + 1) and 
represents the question Q(i, j, k). 
</p> <pre>SAMPLE INPUT
7 3
1 5 2 6 3 7 4
2 5 3
4 4 1
1 7 3

</pre>
<h3>Output</h3>

<pre> 
For each question output the answer to it ¡ª the k-th number in sorted 
a[i ... j] segment. 

SAMPLE OUTPUT
5
6
3
</pre>
<b>Note : naive solution will not work!!!</b>