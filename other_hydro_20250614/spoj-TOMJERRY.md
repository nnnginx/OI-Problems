<p>You may know the great American cartoon called <em>Tom and Jerry</em>. In that cartoon, Tom is a stupid cat, and Jerry is a cute mouse. They are all living in Blue Mary's house. (Maybe the name of the owner of the house they living in is not Blue Mary, but this is not important. ^_^)</p>
<p>One day Jerry gets a GPS, so after that he can detect Tom's position accurately. He decides to play tricks on Tom again. The house has N (1&lt;= N &lt;= 1000) rooms numbered from 1 to n and E(1&lt;= E &lt;=1000) corridors, each connects two different rooms, and there is at most one corridor between two rooms. When Jerry gets the GPS, he is in room No.P(1&lt;= P &lt;=N) while Tom is in room No.Q(1&lt;= Q &lt;= N). You may assume that room No.P and room No.Q is in one connected componenet and they are not the same room. Since Jerry is very cute and Tom is very stupid, if they are in the same room, Jerry can befool Tom as soon as possible. Now Jerry wants to get to Tom's room as soon as possible. At each time unit, he will detect Tom's position, and choose the room next to his room which is the nearest to Tom's position and go to that room. If there are several rooms satisfied the condition above, he will choose the one with the least room number. After that, if they are in the same room, Jerry will stay and play tricks on Tom, or he will repeat this progress one more time otherwise.</p>
<p>Now poor Tom doesn't know he'll be played, he is taking a walk in the house leisurely. Each time unit he will choose a room next to the room he is in and go to that room or stay in the room he is in now, with equal probability. For example, if Tom is now in room 1, room 2 and room 3 are the only neighbors of room 1 (i.e. there is a corridor between room 1 and room 2, and there is a corridor between room 1 and room 3), at the next time unit, the probability of that Tom is in room 1,2 or 3 are all 1/3.</p>
<p>Suppose at each time unit, Jerry moves first, and Tom will move after Jerry complete his move. You task is to calculate the expected time unit from the time when Jerry gets the GPS to the time when Jerry and Tom are in the same room.</p>
<h3>Input</h3>
<p>Multiple test cases, the number of them is given in the very first line.</p>
<p>For each test case:</p>
<p>The first line contains two space-separated integers N and E. The second line contains two space-separated integers P and Q. E lines then follow, each contains 2 space-separated integers A and B which shows that there is a corridor between room A and room B.</p>
<h3>Output</h3>
<p>For each test case:</p>
<p>Output one line, which contains a single real number - the expected time unit, rounded to 3 decimal places.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
4 3
1 4
1 2
2 3
3 4
9 9
9 3
1 2
2 3
3 4
4 5
3 6
4 6
4 7
7 8
8 9

<strong>Output:</strong>
1.500
2.167

</pre>