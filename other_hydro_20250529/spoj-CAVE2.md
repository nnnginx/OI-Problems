<p style="color: #444444; font-family: Tahoma, Arial; font-size: 12.800000190734863px; line-height: 17.600000381469727px;">Byteasar has discovered a cave. It appears that the cave contains n&nbsp;chambers connected with passages in such a way that there exists a single way of getting from any chamber to any other chamber.</p>
<p style="color: #444444; font-family: Tahoma, Arial; font-size: 12.800000190734863px; line-height: 17.600000381469727px;">The cave should now be examined more thoroughly, so Byteasar has asked his friends for help. They have all arrived at the cave and they are willing to divide themselves into groups. Each group should examine the same number of chambers, and each chamber should be examined by exactly one group. Additionally, for the groups not to interfere with each others' work, the members of each group should be able to move between the assigned chambers without passing through chambers assigned to other groups.</p>
<p style="color: #444444; font-family: Tahoma, Arial; font-size: 12.800000190734863px; line-height: 17.600000381469727px;">How many groups can the explorers be divided into?</p>
<h3>Input</h3>
<p style="color: #444444; font-family: Tahoma, Arial; font-size: 12.800000190734863px; line-height: 17.600000381469727px;">The first line of the input contains one integer n&nbsp;(2 ¡Ü n ¡Ü 3000000)&nbsp;denoting the number of chambers in the cave. The chambers are numbered&nbsp;<span><img src="file://hwJGaCnf.png" alt=""></span>&nbsp;through&nbsp;<span><img src="file://fgqr2Wt1.png" alt=""></span>.</p>
<p style="color: #444444; font-family: Tahoma, Arial; font-size: 12.800000190734863px; line-height: 17.600000381469727px;">The following n - 1&nbsp;lines describe connections between the chambers. The i-th of these lines contains an integer a<sub>i</sub>&nbsp;(1 ¡Ü a<sub>i</sub>&nbsp;¡Ü i)&nbsp;which represents a passage connecting chambers number i + 1 and a<sub>i.</sub></p>
<p>&nbsp;</p>
<h3>Output</h3>
<p><span style="color: #444444; font-family: Tahoma, Arial; font-size: 12.800000190734863px; line-height: 17.600000381469727px;">Your program should output a single line containing all integers k</span><span style="color: #444444; font-family: Tahoma, Arial; font-size: 12.800000190734863px; line-height: 17.600000381469727px;">, such that the chambers can be divided into k</span><span style="color: #444444; font-family: Tahoma, Arial; font-size: 12.800000190734863px; line-height: 17.600000381469727px;">&nbsp;disjoint sets of equal size, and one can move between any two chambers belonging to the same set passing only through chambers from this set. The numbers should be written in an ascending order and separated with single spaces.</span></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<pre style="color: #444444; font-size: 12.800000190734863px; line-height: 17.600000381469727px;">6
1
2
3
3
5</pre>
<strong>Output:</strong>
<pre style="color: #444444; font-size: 12.800000190734863px; line-height: 17.600000381469727px;">1 3 6</pre>
<pre style="color: #444444; font-size: 12.800000190734863px; line-height: 17.600000381469727px; text-align: center; "><em>Task author: Jakub Lacki</em></pre>
</pre>