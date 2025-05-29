<p><span style="font-size: medium;">Changu and Mangu are part of a football team which is going to participate in a tournament. In the tournament there are n teams in total. Each team plays twice against every other team (home and away fixture). The team that wins, is awarded 3 points. The team that draws, gets 1 point, while the team that loses gets no points.</span></p>
<p><span style="font-size: medium;">At the end of the tournament, the teams are ranked 1 to n according to total points. <span style="text-align: justify;">The rank of each team&nbsp;</span><em>t</em><span style="text-align: justify;">&nbsp;having&nbsp;</span><em>p</em><span style="text-align: justify;">&nbsp;points is one plus the number of teams having more than&nbsp;</span><em>p&nbsp;</em><span style="text-align: justify;">points. It is possible that more than one team have the same ranks.</span></span></p>
<p style="text-align: justify;"><span style="font-size: medium;">In addition to the team that has rank 1, the&nbsp;<em>Lucky </em>team is also awarded, if it exists. The <em>Lucky&nbsp;</em>team is the one that has absolutely the highest number of wins (absolutely means no other teams has the same number of wins), absolutely the highest number of goals scored, and absolutely the lowest number of goals conceded, is called the <em>Lucky <span style="text-align: justify;">team.&nbsp;</span></em>(<em>Lucky&nbsp;</em>Team should have all these properties.)</span></p>
<p style="text-align: justify;"><span style="font-size: medium;">Changu keeps dreaming about being a part of the Lucky team. Your task is to find out the worst possible rank for the <em>Lucky</em> Team.</span></p>
<p style="text-align: justify;"><strong><span style="font-size: medium;">Input</span></strong></p>
<p><span style="font-size: medium;">The first line contains T, the number of test cases. The next T lines contain a number n, the number of teams participating in the tournament.</span></p>
<p><strong><span style="font-size: medium;">Output</span></strong></p>
<p><span style="font-size: medium;">For each test case, print on a separate line, <span style="text-align: justify;">&nbsp;the worst possible rank for the&nbsp;</span><em>Lucky</em><span style="text-align: justify;">&nbsp;Team</span></span></p>
<p><strong><span style="font-size: medium;">Example</span></strong></p>
<p><strong><span style="font-size: medium;"><strong>Input:</strong></span></strong></p>
<p><span style="font-size: medium;">2</span></p>
<p><span style="font-size: medium;">1</span></p>
<p><span style="font-size: medium;">3</span></p>
<p><span style="font-size: medium;"><strong></strong><span style="font-weight: bold;">Output:</span></span></p>
<p><span style="font-size: medium;">1</span></p>
<p><span style="font-size: medium;">1</span></p>
<p><span style="font-size: medium;"><strong>Constraints:</strong>&nbsp;</span></p>
<p><span style="font-size: medium;">T&lt;=10^5</span></p>
<p><span style="font-size: medium;">1&lt;=N&lt;=10^18</span></p>