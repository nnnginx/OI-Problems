<p align="justify">You are given a list of cities. Each direct connection between two cities has its  transportation cost (an integer bigger than 0). The goal is to find the paths of minimum cost between pairs of cities. Assume that the cost of each path (which is the sum of costs of all direct connections belongning to this path) is at most 200000. The name of a city is a string containing characters a,...,z and is at most 10 characters long.</p>

<h3>Input</h3>
<p align="justify">&nbsp;</p>
<pre><em>s</em> [the number of tests &lt;= 10]
<em>n</em> [the number of cities &lt;= 10000]
<em>NAME</em> [city name]
<em>p</em> [the number of neighbours of city <em>NAME</em>]
<em>nr</em> <em>cost</em> [<em>nr</em> - index of a city connected to <em>NAME</em> (the index of the first city is 1)]
           [<em>cost</em> - the transportation cost]
<em>r</em> [the number of paths to find &lt;= <strong>100</strong>]
<em>NAME1 NAME2</em> [<em>NAME1</em> - source, <em>NAME2</em> - destination]
[empty line separating the tests]
</pre>
<p>&nbsp;</p>

<h3>Output</h3>
<p align="justify">&nbsp;</p>
<pre><em>cost</em> [the minimum transportation cost from city <em>NAME1</em> to city <em>NAME2</em> (one per line)]
</pre>
<p>&nbsp;</p>

<h3>Example</h3>
<p align="justify">&nbsp;</p>
<pre><b>Input:</b>
1
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
2
gdansk warszawa
bydgoszcz warszawa

<b>Output:</b>
3
2
</pre>
<p>&nbsp;</p>
<p><strong>Warning: large Input/Output data, be careful with certain languages</strong></p>