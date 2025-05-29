<p>Your friend came up with an idea of starting a social network-SOCNET.
Since,he is not as good a programmer as you are he needs your help to build certain features.</p>
<p>You need to build an ADD friend feature. if 'x' sends a friend request to 'y',he may accept it or deny it.</p>
<p>SOCNET has a special feature called 'community'.When two people 'x' and 'y' becomes friends,the communities of two are merged together.(If 'x' has no friends,it's community consist of only himself,size-1)</p>
<p>Since,your friend is low on funds,the data center he uses has a restriction-the MAXIMUM size of any community cannot exceed 'm'.</p>
<p>

You need to work on following three types of queries-</p>
<ul>
<li>A x y - x sends a friend request to y</li>
<li>E x y - check whether x and y are present in same community(print 'Yes' or 'No')</li>
<li>S x   - prints the size of the community 'x' belongs to.</li>
</ul>
<p>
NOTE- A friend requested is accepted only if the merger of the two communities results in a community not greater than 'm'.
</p>

<h3>Input</h3>
<p>The first line of input consists of two positive integers - n and m(n is the number of registered users and m is the maximum size of any community).</p>

<p>Next line consist of a positive integer q(number of queries).</p>

<p>q lines follows(Each line consist of a query as described in the problem statement).</p>

<p>The queries follows 1-indexing.</p>

<p></p>

<h3>Constraints</h3>
1&lt;=n,m&lt;=100000,

1&lt;=q&lt;=200000

<h3>Output</h3>
For each query of Type - 'E',output in a single line-'Yes' or 'No'.
For each query of Type - 'S',output the size of the community to which 'x' belongs.
For further clarification,read the example given.


<h3>Example</h3>

<pre><b>Input:</b>
5 3
8
S 2
A 2 3
E 2 3
S 2
A 4 5
A 3 5
E 3 5
S 3


<b>Output:</b>
1
Yes
2
No
2


Explanation-Initially no one has any friend.So community of '2' consist of only '2' i.e size-1. Then '2' and '3' becomes friends .This forms a community of 2 people. '4' and '5' also becomes friends.This forms another community of 2 people. '5' is unable to accept friend request of '3' (because it would result in a community of 4 people(&gt;3).
</pre>