<p>Farmer John's N (1 &lt;= N &lt;= 1000) cows each reside in one of B (1 &lt;= B &lt;= 20) 
barns which, of course, have limited capacity. Some cows really like their 
current barn, and some are not so happy. </p>
<p>FJ would like to rearrange the cows such that the cows are as equally happy 
as possible, even if that means all the cows hate their assigned barn. </p>
<p>Each cow gives FJ the order in which she prefers the barns. A cow's happiness 
with a particular assignment is her ranking of her barn. Your job is to find an 
assignment of cows to barns such that no barn's capacity is exceeded and the 
size of the range (i.e., one more than the positive difference between the the 
highest-ranked barn chosen and that lowest-ranked barn chosen) of barn rankings 
the cows give their assigned barns is as small as possible.</p>


<h3>Input</h3>
<p>Line 1: Two space-separated integers, N and B </p>
<p>Lines 2..N+1: Each line contains B space-separated integers which are exactly 
1..B sorted into some order. The first integer on line i+1 is the number of the 
cow i's top-choice barn, the second integer on that line is the number of the 
i'th cow's second-choice barn, and so on. </p>
<p>Line N+2: B space-separated integers, respectively the capacity of the first 
barn, then the capacity of the second, and so on. The sum of these numbers is 
guaranteed to be at least N.</p>

<h3>Output</h3>
<p>One integer, the size of the minimum range of barn rankings the cows give 
their assigned barns, including the endpoints</p>

<h3>Example</h3>

<pre><b>Input:</b>
6 4
1 2 3 4
2 3 1 4
4 2 3 1
3 1 2 4
1 3 4 2
1 4 2 3
2 1 3 2

<b>Output:</b>
2
</pre>