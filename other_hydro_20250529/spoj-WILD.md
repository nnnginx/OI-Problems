<p>Once upon a time in the west... The quiet life of the villages on the western frontier are often stirred up by the appearance of mysterious strangers. A stranger might be a bounty hunter looking for a notorious villain, or he might be a dangerous criminal escaping the hand of justice. The number of strangers has become so large that they formed the Mysterious Strangers' Union. If you want to be a mysterious stranger, then you have to apply to the Union, and you have to pass three exams that test the three most important skills: shooting, fist-fighting, and harmonica playing. For each skill, the Admission Committeegives a score between 1 (worst) and m (best). Interestingly enough, there are no two members in the Union having exactly the same skills: for every two member, there is always at least one skill for which they have diofferent scores. Furthermore, it turns out that for every possible combination of scores there is exactly one member having these scores. This means that there are exactly m<sup>3</sup> strangers in the union.</p>
<p>Recently, some members left the Union and they formed the Society of Evil Mysterious Strangers. The aim of this group is to commit as many evil crimes as possible, and they are quite successful at it. Therefore, the Steering Committee of the Union decided that a Hero is needed who will destroy this evil society. A Hero is a mysterious stranger who can defeat every member of the Society of Evil Mysterious Strangers. A Hero can defeat a member if the Hero has a higher score in at least one skill. For example, if the evil society has two members, Colonel Bill, with a score of 7 for shooting, 5 for knife throwing and 3 for harmonica playing, and Rabid Jack, with a score 10 for shooting, 6 for knife throwing and 8 for harmonica playing, then a Hero with score 8 for shooting, 7 for knife throwing and 3 for harmonica playing can defeat both ofthem. However, someone with a score of 8 for shooting 6 for knife throwing and 8 for harmonica playing cannot be the Hero. Moreover, the Hero cannot be a member of the evil society.</p>
<p>Your task is to determine whether there is a member in the Union who can be the Hero. If so, thenyou have to count how many members are potential heroes.</p>
<h3>Input</h3>
<p>The input contains several blocks of test cases. Each block begins with a line containing two integers: the number 1 &lt;= n &lt;= 100000 of members in the Society of Evil Mysterious Strangers and the maximum value 2 &lt;= m &lt;= 100000 of the scores. The next n lines describe these members. Each line contains three integers between 1 and m: the scores for the three skills.</p>
<p>The input is terminated by a block with n = m = 0.</p>
<h3>Output</h3>
<p>For each test case, you have to output a single line containing the number of members in the Union who satisfy the requirements for becoming a Hero. If there is no such member, then output <em>0</em>. It can be assumed that the output is always at most 10<sup>18</sup>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3 10
2 8 5
6 3 5
1 3 9
1 3
2 2 2
1 10000
2 2 2
0 0

<strong>Output:</strong>
848
19
999999999992
</pre>
<p><strong>Warning: enormous input/output data, be careful with certain languages</strong></p>