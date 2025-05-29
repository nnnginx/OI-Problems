<p><span style="font-size: small;"> You are given <strong>n</strong> cities with <strong>m</strong> bi-directional roads connecting them and the   length of each road. There are two friends living in different cities who wish   to collect some ingredients available at different stores to make cake. There   are s such stores. They need not come back home after purchasing the   ingredients. Petrol is expensive and they would hence like to travel minimum   total distance (sum of distance distance traveled by both kids). Help them   find out what this distance is. </span></p>
<h3><span style="font-size: small;">Input Format:</span></h3>
<p><span style="font-size: small;"><strong>n m</strong><br> (<strong>m</strong> lines of the form <strong>a<sub>i</sub> b<sub>i</sub> c<sub>i</sub></strong>)<br> Here <strong>n</strong> is number of cities, <strong>m</strong> is number of roads, <strong>a<sub>i</sub></strong> and <strong>b<sub>i</sub></strong> are the cities(0   indexed) the roads connect and <strong>c<sub>i</sub></strong> is the length of this road<br> <strong>s</strong> where <strong>s</strong> is the number of stores<br> (1 line containing <strong>s</strong> space separated integers indicating the city number in   which the stores are located.)<br> (two space separated integers indicating the cities in which the two kids   live) </span></p>
<h3><span style="font-size: small;">Output Format:</span></h3>
<p><span style="font-size: small;"> Single integer <strong>x</strong> where <strong>x</strong> is the minimum distance that the duo will travel that   is minimum sum of distance travelled by first kid and second kid. </span></p>
<h3><span style="font-size: small;">Constraints:</span></h3>
<p><span style="font-size: small;"><strong> 2 ¡Ü n ¡Ü 100<br> 1 ¡Ü m ¡Ü (n*(n-1))/2<br> 0 ¡Ü a,b &lt; n<br> 0 ¡Üc¡Ü 1000<br> 1 ¡Ü s ¡Ü 8<br></strong> </span></p>
<h3><span style="font-size: small;">Sample Input:</span></h3>
<pre><span style="font-size: small;">5 6
0 1 5
1 4 1
0 4 10
0 2 2
1 2 3
2 3 4
2
2 4
0 1</span></pre>
<h3><span style="font-size: small;">Sample Output:</span></h3>
<pre><span style="font-size: small;">3</span></pre>
<p><span style="font-size: small;"><br> <strong>Problem Setter: Vidit Gupta</strong></span></p>