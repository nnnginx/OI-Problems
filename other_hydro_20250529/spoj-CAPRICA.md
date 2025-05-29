<p>Caprica is one of the 12 colonial planets, but it was completely destroyed by the cylons, robots made<br>by humans that had rebelled. Before the attack, Doctor Gaius Baltar had the following problem.<br>Caprica has N cities, numbered from 0 to N − 1, and M bidirectional roads connecting them, in<br>a way that exists a path between every pair of cities. Let X and Y be two disjoint and non-empty<br>subsets of this N cities. The problem is to find the smallest path length between any cities x and y<br>where x ∈ X and y ∈ Y . A path length is the sum of the distance of each road in this path.</p>
<h3>Input</h3>
<p>Each test case is described using several lines. The first line contains four integers N , M , A and B<br>representing respectively the number of cities (2 ≤ N ≤ 1000), the number of roads (1 ≤ M ≤ 10<sup>4</sup> ),<br>the number of cities in X (2 ≤ A ≤ 1000), and the number of cities in Y (2 ≤ B ≤ 1000), where<br>A + B ≤ N.<br>The second line contains A integers and the third line contains B integers, representing the cities<br>in X and Y respectively. Each of the next M lines describes a road using three integers, u, v, and d,<br>indicating that there is a road between the cities u and v with distance d (1 ≤ d ≤ 10<sup>4</sup> ).<br>The last test case is followed by a line containing four zeros.</p>
<h3>Output</h3>
<p>For each test case output, in a single line, the integer representing the smallest path length between<br>x and y where x ∈ X and y ∈ Y .</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4 4 2 2<br>0 1<br>2 3<br>0 1 10<br>0 2 20<br>1 3 10<br>2 3 10<br>0 0 0 0<br><br><strong>Output:</strong>
10
</pre>