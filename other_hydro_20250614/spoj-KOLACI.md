<p>Darko and Marko are twins and they love to eat cookies. Their grandma Mara loves to bake cookies, but she doesn't like the fact that Darko and Marko eat them too fast.</p>
<p>To teach her grandsons to eat slower, Mara turned it into a game. Mara will bake N cookies and assign them with integers 1 to N. Then she will arrange them in a circle such that each cookie i is between to cookie i−1 and i+1 except for cookies 1 and N that are neighbors.</p>
<p>Mara knows a recipe for 26 different types of cookies. We will denote a cookie type with lower case english letters 'a' to 'z'.</p>
<p>Darko and Marko will each get one cookie every 5 minutes. Mara will say one integer out loud. Darko and Marko will search for a cookie with this number, but will eat two neighboring cookies. This procedure is repeated until one or two cookies are left on the table. Then the game ends and Mara eats the remaining cookies.</p>
<p><img style="border: 0px initial initial;" src="../../content/kalinov:kolaci" alt="" width="620" height="198"></p>
<p>The game can be represented with a sequence of (N−1) div 2 integers that Mara said out loud. For example, the illustrations above can be represented with a sequence (4, 8, 6). Two games are considered different if their respective sequences are different.</p>
<p>After a few games Mara noticed that Marko and Darko often fight during the game. In fact, they fight every time when the two neighboring cookies are of different types because they can't decide which one will get which cookie.</p>
<p>Mara decided to count the number of ways to play a game in a way to avoid such situations.</p>
<p>Given a cookie type for each of N cookies, write a program that will calculate the number of ways to play a game such that Darko and Marko will not fight. This number can get very large, so output the remainder of division by 10007 instead.</p>
<h3>Input</h3>
<p>The first line contains one integer N (3 ≤ N ≤ 75), the number of cookies.</p>
<p>The second line contains a sequence of N lower case english letters, types of cookies in order they are arranged in a circle.</p>
<h3>Output</h3>
<p>Output a single integer, the total number of ways to play a game that will prevent Darko and Marko from fighting modulo 10007.</p>
<h3>Example</h3>
<table style="width: 100%;" border="0" frame="void" align="center">
<tbody>
<tr>
<td align="left" valign="top">
<pre><strong>Input:</strong>
8
cibaboca

<strong>Output:</strong>
4</pre>
</td>
<td align="left" valign="top">
<pre><strong>Input:</strong>
5
aabab

<strong>Output:</strong>
5</pre>
</td>
<td align="left" valign="top">
<pre><strong>Input:</strong>
11
fffffffffff

<strong>Output:</strong>
388</pre>
</td>
</tr>
</tbody>
</table>
<p>Clarification for the first example: This sample corresponds to illustration above. Four valid sequences are (4, 8, 2), (4, 8, 6), (8, 4, 2) i (8, 4, 6).</p>
<p>Clarification for the second example: Five valid sequences are (3, 1), (5, 2), (4, 4), (4, 1) i (4, 2).</p>
<p>Clarification for the third example: All cookies share the same type, so Darko and Marko can't get into fight no matter what. In each step Mara can say any integer remaining on the table, so the total number of games is equal to 11⋅9⋅7⋅5⋅3 = 10395. 388 is the remainder of division by 10007.</p>