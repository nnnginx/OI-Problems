<p>Given a sequence of 12 numbers consisting of 0 and the first 11 natural numbers. Suppose number 0 is in the i-th position of the sequence (positions are numbered from 0 to 11). You can swap it with the number in the j-th position if the following conditions hold:
</p><ul>
<li>| i ¨C j | = d<sub>k</sub> , where k=1..3 and (d<sub>1</sub>,d<sub>2</sub>,d<sub>3</sub>,d<sub>4</sub>)=(1;3;6;12)
</li><li>
floor(i/d<sub>k+1</sub>)=floor(j/d<sub>k+1</sub>)
</li></ul>
<p>
Your task is to find the minimum number of exchange operations required to sort the sequence in increasing order.
</p><h3>Input</h3>
<p>The first line of the input file contains an integer representing the number of test cases to follow.
Each test case contains a sequence of twelve numbers consisting of 0,1,2,..,11, separated by single space.
You can assume that the given sequence can always be sorted in increasing order by using the exchange operations 
</p><h3>Output</h3>
<p>For each test case, output the minimum number of exchange operations required to sort the given sequence in increasing order.
</p><h3>Example</h3>

<pre><b>Input:</b>
2
1 10 2 3 0 5 7 4 8 6 9 11
6 4 1 0 3 5 9 7 2 10 11 8

<b>Output:</b>
8
9
</pre>