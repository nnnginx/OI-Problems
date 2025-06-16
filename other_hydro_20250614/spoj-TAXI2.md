<p>In Berland a new movie was released on the occassion of 14th Feb. The craze for this movie was very much among the peoples of the city. So many of them decided to go to the only Movie Theatre of Berland. As berland is very much developed there are many large(tall) buildings, including the movie theatre. At each building except theatre, there exist a person (who wants to see movie) or a taxi driver with his taxi. As it is very late in the night each taxi driver will only accomodate only one passenger and also he will only drive for <strong>T[i]</strong> HRS (return journey is not included). You will be given the distance between building <strong>D[i]</strong> and the speed of each taxi driver <strong>S[i]</strong>. As I am the owner of this theatre help me by telling, the maximum number of people I will see in the theatre for the movie. <strong>N+P+1</strong>th building is the my theatre. Also, if a taxi starts his journey by taking a passenger, it only stops at the theatre.</p>
<h3>Input</h3>
<ul>
<li>First line contains <strong>TT</strong> the number of test cases.</li>
<li>First line of each test test case contains <strong>N</strong>, <strong>P</strong> and <strong>R</strong> denoting the number of taxi, number of people, and the number of roads between buildings.</li>
<li>Next line contains <strong>N</strong> space-seperated integers representing the building where taxi is present.</li>
<li>Next line contains <strong>P</strong> space-seperated integers representing the building where passengers is present.</li>
<li>Next <strong>R</strong> lines contains <strong>X</strong>, <strong>Y</strong>, and <strong>D[i]</strong> the building connected via road and the distance between them in KMs.</li>
<li>Next line contains <strong>N</strong> space-sperated integers <strong>S[i]</strong> giving the speed details of each taxi in KM/HRs.</li>
<li>Next line contains <strong>N</strong> space-sperated integers <strong>T[i]</strong> giving the time details of each taxi in HRs.</li>
</ul>
<h3>Output</h3>
<ul>
<li>Maximum number of people that will visit my theatre.</li>
</ul>
<h3>Constraints&nbsp;</h3>
<ul>
<li><strong>1</strong> &lt;= <strong>TT</strong> &lt;= <strong>5</strong></li>
<li><strong>1</strong> &lt;= <strong>N</strong> &lt;= <strong>500</strong></li>
<li><strong>1</strong> &lt;= <strong>P</strong> &lt;= <strong>1000</strong></li>
<li><strong>1</strong> &lt;= <strong>R</strong> &lt;= <strong>50000</strong></li>
<li><strong>1</strong> &lt;= <strong>X</strong>, <strong>Y</strong> &lt;= <strong>N</strong></li>
<li><strong>5</strong> &lt;= <strong>S[i]</strong> &lt;= <strong>50</strong></li>
<li><strong>1</strong> &lt;= <strong>T[i]</strong> &lt;= <strong>5</strong></li>
<li><strong>1</strong> &lt;= <strong>D[i]</strong> &lt;= <strong>100</strong></li>
</ul>
<ul>
</ul>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
1 2 4
2
1 3
1 2 5
2 3 5
3 4 10
1 3 8
20
1

<strong>Output:</strong>
1
</pre>