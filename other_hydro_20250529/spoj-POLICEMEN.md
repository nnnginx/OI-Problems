<p>There is a country of <em>n </em>cities and <em>n-1</em> bidirectional roads you can go from any city to another using its roads</p>
<p>You are a police man and there is a theif who is going to escape from the country using an airport in city 1 you are given <em>m</em> queries which of type "<em>a b"</em> which means the thief is in city <em>a</em> and you are in city <em>b</em> you should find if it's possible to catch him before he escape or not and find the city which you will catch him in if it's possible.</p>
<p>You are moving at the same speed the thief moving at and the thief is taking the shortest path to city 1</p>
<p>If you arrived in a city in the same time as the thief you can catch him in it if you arrived before him you can wait for him</p>
<p>If there is more than one city you can catch him in print the nearest one to you.</p>
<h3>Input</h3>
<p>the first line contains an integer <em>n</em> (<em>1 <em>¡Ü </em>n <em>¡Ü </em>10<sup>4</sup></em>)&nbsp; then <em>n-1</em> lines each contains two integers which means there is a road between city <em>u</em> and <em>v</em></p>
<p>then an intger <em>q</em> (<em>1 ¡Ü q <em>¡Ü</em> 10<sup>4</sup></em>)<em> </em>and <em>q</em> lines of form a b (<em><em>1 ¡Ü</em> a , b <em>¡Ü </em>n</em>) which are the thief's position and your position</p>
<h3>Output</h3>
<p>for each query print YES then a space then the city which you will catch him in if it's possible otherwise print NO</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5<br>1 2<br>1 3<br>2 4<br>4 5<br>4<br>1 2<br>1 1<br>5 4<br>2 3<br><strong>Output:</strong>
NO<br>YES 1<br>YES 4<br>YES 1</pre>