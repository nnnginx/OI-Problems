<p>Do you know the famous game THE KING OF FIGHTERS? If the answer is yes, I'm sure you know THE THREE BLACK GROUP: Chris, Shermie and Yashiro. Today Chris is invited to one of his friends' home to play THE KING OF FIGHTERS.Blue Mary is now at Chris' home, she knows where Shermie's and Yashiro's home is, but she doesn't know where Chris actually is.So she decides that:
</p><div align="justify">
       <ul>
               <li>
               If Yashiro's home is nearer than Shermie's, she will go to Yashiro's home first, if she doesn't find Chris, she will then go to Shermie's, and vice versa.
               </li><li>
               The map of the city is strange. Each of the houses is assigned to a unique number in the range[1,n], where n is the number of houses. Between some pairs of houses there are some roads. There exists one and only one path from any house to any other house. She will go along the only path between the two houses.</li>
       </ul>
</div>
<p>Unfortunately, you don't know where Chris' home actually is, and the same as Yashiro's and Shermie's. Now you are interesting in the maximum time from the time when Blue Mary starts from Chris' home to the time when Blue Mary finds Chris in the worst case.</p>
<h3>Input</h3>
<p>The number of test cases T is given in the very first line.T blocks follow.</p>
<p>For each test case, the first line contains 2 space-separated integers N(3&lt;=N&lt;=200000) and M, which denotes the number of houses and the number of roads in the city.M lines follow, each contains 3 space-separated integers x,y,z(1&lt;=x,y&lt;=n,1&lt;=z&lt;=10<sup>9</sup>).It tells us there exist a road between house No.x and house No.y, and to go from x to y or from y to x along this road will take z minutes.No two roads are repeated.</p>
<h3>Output</h3>
<p>For each test case you should output a single line, which contains a single integer - the maximum time measured in minutes.</p>
<h3>Example</h3>
<pre><b>Input:</b>
1
4 3
1 2 1
2 3 1
3 4 1

<b>Output</b>
4
</pre>
<b>Warning: large Input/Output data, be careful with certain languages</b>