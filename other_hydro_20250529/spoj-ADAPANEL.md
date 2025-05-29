<p> Ada the Ladybug has proved succesful in solving some hard problems, so a construction
company has asked her to solve a problem for them. There are multiple cities in
the country and each city owns exactly one panel-block. There are also
unidirectional roads between some pairs of cities (note that circular
self-roads and multi-roads with several traffic lines are allowed). A city can
sell its panel-block to any city, to which they could transport the panel
block, and from which they can bring back their reward for it (i.e. there must
be a path from actual city to destination city and back). As long a city has
<b>K</b> panel-blocks, it builds a prefab of height <b>K</b> which looks exactly
same as each other prefab of height <b>K</b>.

<!--<p>They are wondering, how many distinct structures (sets of prefabs) might arise. Anyway
note, that any permutation of structures in a set of cities, from which you can
get to each other is considered same, since it would be too easy to make some
shuffling. But this doesn't apply to cities from other sets!  -->

</p><p>The construction company notes all the heights down and puts them in an array. They are wondering how many distinct arrays are possible by moving the panel blocks between cities. However there is a catch. Consider a set of cities in which each city is reachable by every other city. Since we can easily shuffle the panel blocks between such a set of cities, we can create new permutations with the same set of heights. The construction company will NOT count any such cases. Hence they will only consider the distinct set of heights for such a set of cities.

</p><p>You have proved succesful in helping Ada with some hard problems, so she has
asked you to help her. Your job is following - count the number of possible
structures which could arise. Since this number might be pretty big, you have to
output it modulo <b>10<sup>9</sup>+7</b>.




</p><h3>Input</h3>

<p>The first line contains two integers <b> 1 ¡Ü N, M ¡Ü 2*10<sup>5</sup></b>,
the number of cities  an the number of unidireectional roads between them.

</p><p> The next <b>M</b> lines contains two integers <b>0 ¡Ü a, b &lt; N</b>,
the road from city <b>a</b> to city <b>b</b>

</p><h3>Output</h3>

Print a single line - the number of possible structures modulo
<b>1000000007</b>.

<h3>Example Input</h3>
<pre>7 9
0 1
1 2
2 3
3 1
2 0
4 5
5 4
6 4
5 6
</pre>
<h3>Example Output</h3>
<pre>15
</pre>
<h3>Example Input 2</h3>
<pre>7 7
0 1
1 2
2 3
3 4
4 5
5 6
6 0
</pre>
<h3>Example Output 2</h3>
<pre>15
</pre>
<h3>Example Input 3</h3>
<pre>6 3
0 1
3 2
4 5
</pre>
<h3>Example Output 3</h3>
<pre>1
</pre>
<h3>Example Input 4</h3>
<pre>8 7
0 1
1 0
2 3
3 2
4 5
5 6
6 4
</pre>
<h3>Example Output 4</h3>
<pre>12
</pre>