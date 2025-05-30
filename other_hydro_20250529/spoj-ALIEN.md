<p>
The aliens have arrived to Earth and everything is in harmony, the two races can live together. However, one specific Female Alien does not want to see humans on her way to the university, the alien must use the train as every human does. But she can choose any train station such she doesn��t see more than B humans, however, the Alien wants to go as far as possible with the train. Please, help her in this task.
</p>

<h3>Input</h3>
<p>
You will receive one integer T denoting the number of test cases, then, the next line will contain two integers At Bt where At and Bt is the number of stations in the train (1 &lt;= At &lt;= 100,000) and the number of people that the alien wants to see as maximum (1 &lt;= Bt &lt;= 10,000,000), after that, one line containing At integers separated by a single space will denote the number of people the Alien can find in the At-i-th station. (For each station there will be as much 100 people)
</p>

<h3>Output</h3>
<p>
Your output should consist on T pair of numbers denoting the number of people the alien will see and the number of stations she will pass respectively.
</p>

<h3>Example</h3>
<pre><strong>INPUT:</strong>
1
5 100
20 15 30 80 100

<strong>OUTPUT</strong>
65 3</pre>

<p><b>Output note:</b><br>
The alien takes the train at station 1 (with 20 people) and goes to station 2, then the 3rd station, at this point, she have seen 65 people, if she decides to go to station 4 she will see 145 people�� Then she exits the station.</p>

<p>The alien, however, can start at station 2 with 15 people, then continue up to the 4th station, then, she would have seen 125 people, but, as she wants to see the minimum people possible and this number of people exceeds what she wants to see, she decides to choose the way from the 1st to the 3rd station.</p>

<p><strong>Clarification: </strong>The alien will be moving always forward (remember, she can choose any station as a start), NEVER backwards, and you should choose the <span style="text-decoration: underline;">best</span> path that satisfies the output specification.</p>