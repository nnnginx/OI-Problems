<p>For the organizers of a soccer world championship the final draw is a very delicate job. It determines the compositions of the groups for the first stage of the tournament and indirectly also the possible matches in the knockout stage. The importance lies in the fact that the success of a team might depend on the opponents it faces - and, maybe, even the winner of the tournament.</p>
<p>The final draw is often subject to accusations of fraud. Some teams tend to think that their group is stronger than others and therefore complain they were cheated. Your job is to provide some facts that can help convince them of the opposite.</p>
<p>The draw is somewhat complicated due to a number of fairness considerations. The objective is not to assign too many good teams to the same group. Also teams from the same confederation should be drawn into different groups. This is ensured by the following rules.</p>
<ul>
<li>There are <em>g</em> groups with <em>m</em> members each. </li>
<li>The hosting nation will be seeded first in the first group.</li>
<li><em>g-1</em> selected teams will be seeded first in the remaining groups.</li>
<li>The remaining positions are drawn from <em>m-1</em> pots, one team from each pot per group.</li>
<li>You will be told which teams belong to the same confederation and you have to ensure that no two teams of the same confederation are in the same group. For confederations with more than <em>g</em> teams this is impossible, so for these confederations you can ignore this rule.</li>
<li>You may assume that for confederations with at most <em>g</em> teams, all teams of the confederation which are not seeded are in the same pot.</li>
<li>Note that each team belongs to exactly one confederation and each team is either seeded or contained in exactly one pot.</li>
</ul>
<p>We want to compute the average strength of the opponents of a given team. The strengths of the teams will be given in the input. Now you have to compute the average of the sum of the strengths of the other teams in the group of the given team. The average is evaluated over all correct draws which are assumed to have the same likelihood.</p>
<h3>Input</h3>
<p>The input starts with the number of test cases. Each test case is described as follows.</p>
<p>The first line contains the number of groups <em>g �� 8</em> and the number of teams per group <em>m �� 4</em>. A line with <em>g * m</em> integers follows. The <em>i</em>-th integer <em>0 �� s<sub>i</sub> �� 10000</em> denotes the strength of the <em>i</em>-th team.</p>
<p>The team indices start from <em>0</em>. By convention, the hosting nation is assigned number <em>0</em>. The next line lists the <em>g-1</em> seeded teams by their numbers. Each of the <em>m-1</em> following lines contains <em>g</em> teams which are allocated to the same pot.</p>
<p>The next line specifies the number of confederations <em>c</em>. <em>c</em> lines follow which describe one confederation each. Each confederation description starts with the number of teams <em>n<sub>i</sub> &gt; 0</em>. Then <em>n<sub>i</sub></em> numbers with the team indices follow.</p>
<p>The last line contains the number <em>t</em> of the team, whose average group strength has to be evaluated.</p>
<h3>Output</h3>
<p>Output the average of the sum of strengths of the opponents of team <em>t</em> in the group stage with 3 decimals on a single line.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
2 3
1 2 3 4 5 6
1
2 5
3 4
1
6 0 1 2 3 4 5
5
2 3
1 2 3 4 5 6
1
2 5
3 4
2
2 0 5
4 1 2 3 4
5

<strong>Output:</strong>
6.000
6.500
</pre>