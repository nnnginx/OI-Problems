<p>Ada the Ladybug is a well know farmer. As she has experience with building fences and breeding animals, she was asked by leader of local zoo - Lichsteiner Leech - to help them design a paddock for animals.</p>
<p>The problem is following: The zoo breeds very rare beasts called Tyg3Rs. There are few of them in a <strong>N x N</strong> square paddock with squares have different heights. The Tyg3Rs live in (little) sqares and the breeders want them to play with each other. At first it is not possible to travel between distinct squares, but it is possible to connect any two adjacent squares for cost of absolute difference of their heights (by making slope).</p>
<p>Now, for each subset of Tyg3Rs, the zoo wants to know minimal price to connect the squares in such way, that each Tyg3R can get to each other. As the output would be pretty big, they just want you to sum these costs.</p>
<p>As her good friend (and as the instances are too big for her to handle), she has asked you to help her with this problem.</p>
<h3>Input</h3>
<p>The first line contains <strong>T</strong>, the number of test-cases.</p>
<p>The first line of each test-case contains <strong>2 ¡Ü N ¡Ü 17</strong>, the size of big square.</p>
<p>Each of the next <strong>N</strong> lines contain <strong>N</strong> integers, the heigths of each square. Each number is between <strong>0</strong> and <strong>1000</strong>.</p>
<p>The next line contains <strong> 1 ¡Ü Q ¡Ü 10</strong>, the number of Tyg3Rs.</p>
<p>The next <strong>Q</strong> lines contains two integers: <strong>0 ¡Ü x, y &lt; N</strong>, the coordinates of Tyg3Rs. Note that multiple Tyg3Rs might already live in the same square.</p>
<h3>Output</h3>
<p>For each test-case print the sum of costs of cheapest way to connect all subset of Tyg3Rs.</p>
<h3>Example Input</h3>
<pre>4
3
1 2 1
2 1 2
1 2 1
3
0 0
0 2
2 1
3
5 5 5
7 5 5
3 4 4
4
0 0
0 0
0 0
2 0
3
1 2 3
4 5 6
7 8 9
2
0 0
2 2
8
1 8 5 2 3 6 7 4
1 5 7 5 4 6 8 7
9 8 7 4 5 2 3 6
1 4 5 7 2 5 3 6
5 2 1 2 4 5 8 5
9 9 9 9 6 6 4 5
2 2 3 4 9 1 9 1
1 4 1 4 7 5 2 1
5
0 0
5 6
3 3
2 1
7 7
</pre>
<h3>Example Output</h3>
<pre>12
14
8
441
</pre>
<h3>Input Explanation</h3>
<p>Prices of subsets of first test-case</p>
<pre>000: 0
100: 0
010: 0
001: 0
110: 2
101: 3
011: 3
111: 4
</pre>
<p>For the second test-case, each subset costs 0, unless those, which consists of last Tyg3R (and some other) - those cost 2.</p>
<p>The third test-case has only one valuable subset (of both Tyg3Rs), which goes on top/right border, and costs 8.</p>