<p>A road network in a country consists of N cities and M one-way roads. The cities are numbered 1 through N. For each road we know the origin and destination cities, as well as its length.</p>

<p>We say that the road F is a continuation of road E if the destination city of road E is the same as the origin city of road F. A path from city A to city B is a sequence of road such that origin of the first road is city A, each other road is a continuation of the one before it, and the destination of the last road is city B. The length of the path is the sum of lengths of all roads in it.</p>

<p>A path from A to B is a shortest path if there is no other path from A to B that is shorter in length.</p>

<p>Your task is to, for each road, output how many different shortest paths containing that road, modulo 1 000 000 007.</p>

<h3>Input</h3>
<p>The first line contains two integers N and M (1 ¡Ü N ¡Ü 1500, 1 ¡Ü M ¡Ü 5000), the number of cities and roads.</p>

<p>Each of the following M lines contains three positive integers O, D and L. These represent a one-way road from city O to city D of length L. The numbers O and D will be different and L will be at most 10000.</p>

<h3>Output</h3>
<p>Output M integers, each on its own line ¨C for each road, the number of different shortest paths containing it, modulo 1 000 000 007. The order of these numbers should match the order of roads in the input.</p>


<h3>Example</h3>

<pre><b>Input:</b>
4 4
1 2 5
2 3 5
3 4 5
1 4 8

<b>Output:</b>
2
3
2
1

<b>Input:</b>
5 8
1 2 20
1 3 2
2 3 2
4 2 3
4 2 3
3 4 5
4 3 5
5 4 20

<b>Output:</b>
0
4
6
6
6
7
2
6
</pre>

<p>Note: The test data for this problem consist of the official test cases from the contest, as well some cases of my own.</p>