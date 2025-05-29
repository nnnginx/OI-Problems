<p>In Hanoi, there are N beauty-spots (2 &lt;= N &lt;= 200), connected by M one-way streets. The length of each street does not exceed 10000. You are the director of a travel agency, and you want to create some tours around the city which satisfy the following conditions:
</p><ul>
<li> Each of the N beauty-spots belongs to exactly one tour.
</li><li> Each tour is a cycle which consists of at least 2 places and visits each place once (except for the place we start from which is visited twice). 
</li><li> The total length of all the streets we use is minimal.
</li></ul>
<h3>Input</h3>
<p>The first line of input contains the number of testcases t (t &lt;= 15). The first line of each testcase contains the numbers N, M. The next M lines contain three integers U V W which mean that there is one street from U to V of length W. 
</p><h3>Output</h3>
<p>For each test case you shold output the minimal total length of all tours.
</p><h3>Example</h3>

<pre><b>Input:</b>
2
6 9
1 2 5
2 3 5
3 1 10
3 4 12
4 1 8
4 6 11
5 4 7
5 6 9
6 5 4
5 8
1 2 4
2 1 7
1 3 10
3 2 10
3 4 10
4 5 10
5 3 10
5 4 3

<b>Output:</b>
42
40

<b>Detailed explanation:</b>
Test 1:
  Tour #1:  1 - 2 - 3 - 1  --&gt; Length = 20
  Tour #2:  6 - 5 - 4 - 6  --&gt; Length = 22

Test 2:
  Tour #1:  1 - 3 - 2 - 1  --&gt; Length = 27
  Tour #2:  5 - 4 - 5      --&gt; Length = 13

</pre>