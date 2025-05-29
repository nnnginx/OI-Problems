<p>You, the wisest minion in town, is selecting a magic school for your brother Stuart to enroll in the coming year. There are N magic school in Fabulous-Imagination Town (FIT). Each school teaches either blue magic or white magic. There are N-1 bidirectional roads between the schools, each road connecting two different schools. Schools are connected in such a way, that there exists a unique path between any two schools.</p>
<p>You plan to visit some of the schools. Each school has a happiness factor, by which your overall happiness increases when you visit the school. Note that if the happiness factor is negative, your overall happiness decreases.</p>
<p>To plan your trip, you choose two different schools, the departure and destination school. You will visit all the schools on the path between the departure and the destination schools, both of them including. To keep things in balance, you must visit the same number of white magic schools as blue magic schools.</p>
<p>You are now wondering, what is the optimal trip that maximize the happiness of the trip, i.e. sum of the happiness factors of the schools you visit.</p>
<p>Given the description of schools and connections between them, Find the optimal trip around the schools, in which you visit the same number of blue and while magic schools and the happiness of the trip is as large as possible.</p>
<h3>Input</h3>
<p>Input consists of four lines.</p>
<p>First line contains a single integer N (2&lt;=N&lt;=10^5), number of schools (schools are numbered from 1 to N).</p>
<p>Second line contains a string of length N, consisting of "B" and "W" characters. If the i-th character is "B", then the i-th school is teaching blue magic. If the i-th character is "W", then the i-th school is teaching white magic. There will be at least one school teaching white magic ad at least one school teaching blue magic.</p>
<p>Third line contains N space-separated integers h_1,h_2,...h_N (-10^5 &lt;= h_i &lt;= 10^5). Integer h_i is the happiness factor of the i-th school.</p>
<p>Fourth line contains N - 1 space-separated integers v_1, v_2, ..., v_(N-1). Integer v_i means there is a road connecting the schools with numbers v_i and (i+1) (1&lt;=v_i&lt;=i).</p>
<h3>Output</h3>
<p>Output exactly one integer, maximum overall happiness of the trip, in which you visit the same number of blue and white magic schools.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
6</pre>
<pre>BWBBBW</pre>
<pre>6 0 3 -2 100 5</pre>
<pre>1 2 2 4 4

<strong>Output:</strong>
9</pre>
<pre><strong><em>Note:</em></strong> In the optimal trip you visit the schools 1,2,4,6.</pre>