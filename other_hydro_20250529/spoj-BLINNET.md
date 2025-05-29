<p align="justify">
<i>We have discovered the fastest communication medium </i> Bytelandian scientists announced, and they called it <i>blingors</i>.
The blingors are incomparably better than other media known before. Many companies in Byteland started to build blingors networks, so the information society in the kingdom of Bytes is fact!
The priority is to build the core of the blingors network, joinig main cities in the country. 
Assume there is some number of cities that will be connected at the beginning. The cost of building blingors connection between two cities depends on many elements, but it has been successfully estimated. 
Your task is to design the blingors network connections between some cities in this way that between any pair of cities is a communication route.  The cost of this network should be as small as possible.
</p>
<p>Remarks</p>
<div align="left">
<ul>
  <li>The name of the city is a string of at most 10 letters from <i>a,...,z</i>.
  </li><li>The cost of the connection between two cities is a positive integer. </li><li>The sum of all connections is not greater than 2<sup>32</sup>-1.
  </li><li>The number of cities is not greater than 10 000. </li></ul></div>
<h3>Input</h3>
<pre><p align="justify">
<br><i>s</i> [number of test cases &lt;= 10]
<i>n</i> [number of cities &lt;= 10 000]
<i>NAME</i> [city name]
<i>p</i> [number of neigbouring cities to the city <i>NAME</i>]
<i>neigh</i> <i>cost</i> 
     [<i>neigh</i> - the unique number of  city from the main list
      <i>cost</i> - the cost of building the blingors connection from <i>NAME</i> to <i>neigh</i>]
[empty line between test cases]
</p>
</pre>
<h3>Output</h3>
<p align="justify">
[separate lines]
<i>cost</i> [the minimum cost of building the blingors network]</p>
<h3>Example</h3>
<pre><b>Input:</b>
2

4
gdansk
2
2 1
3 3
bydgoszcz
3
1 1
3 1
4 4
torun
3
1 3
2 1
4 1
warszawa
2
2 4
3 1

3
ixowo
2
2 1
3 3
iyekowo
2
1 1
3 7
zetowo
2
1 3 
2 7


<b>Output:</b>
3
4
</pre>
<b>Warning: large Input/Output data, be careful with certain languages</b>