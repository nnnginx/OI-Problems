<p>Jolly Kingdom is a kingdom which is famous for its troops' power. Jolly Kingdom has N swordsman troops and M archer troops where each troop has his/her own unique fighting style, different with others.</p>
<p>For the 10<sup>th</sup> times, an evil witch with her monster troops tries to seize the throne of Jolly Kingdom. According to the information gathered from Jolly Kingdom's spies, the witch will attack everyday for H days. Each day, the witch will add 1 new monster into her monster troops. This makes enemy's troops become stronger every day.</p>
<p>Each monster owned by the witch is strong and almost unbeatable, only the X<sub>i</sub><sup>th</sup> swordsman troop or the Y<sub>i</sub><sup>th</sup> archer troop can beat the monster. After the monster has been defeated by Jolly Kingdom's troop, that monster will take a reset and attack again in the next day.</p>
<p>To protect Jolly Kingdom, every day <strong>all monsters</strong> have to be defeated, but the cost to send 1 troop is expensive, so the king wants to send minimum number of troops every day such that the sent troops will be able to defeat <strong>all monsters</strong> exist on that corresponding day.</p>
<p>The king asks you for your help, as a royal advisor, the number of troops the king has to send every day.</p>
<p>&nbsp;</p>
<p><strong>Input</strong></p>
<p>First line consists of 3 integers: N, M, and H (1 ¡Ü N, M ¡Ü 1000; 1 ¡Ü H ¡Ü N*M) ¨C the number of swordsman troops, archer troops, and days. Each of next H lines contains 2 integers: X<sub>i</sub> and Y<sub>i</sub> (1 ¡Ü X<sub>i</sub> ¡Ü N; 1 ¡Ü Y<sub>i</sub> ¡Ü M) ¨C the weakness of i<sup>th</sup> monster, i<sup>th</sup> can be defeated by the X<sub>i</sub><sup>th</sup> swordsman or Y<sub>i</sub><sup>th</sup> archer.</p>
<p>There can't be 2 monsters with the exact same weakness (there won't be any monster i and j where X<sub>i</sub> = X<sub>j</sub> and Y<sub>i</sub> = Y<sub>j</sub> for all 1 ¡Ü i, j ¡Ü H and i ¡Ù j).</p>
<p>&nbsp;</p>
<p><strong>Output</strong></p>
<p>Print H lines. Each line contains 1 number represents the answer to the king's question.</p>
<p>&nbsp;</p>
<p><strong>Sample Tests</strong></p>
<!-- ngRepeat: input in problemDetails.sampleInput track by $index --> 
<table class="table table-striped ng-scope" border="0">
<tbody>
<tr style="background-color: #cccccc;">
<td class="tableHeader">Input</td>
</tr>
<tr style="background-color: #eeeeee;">
<td>
<pre class="ng-binding">4 4 9
1 1
1 2
1 3
2 1
4 1
3 4
3 3
4 3
4 4
</pre>
</td>
</tr>
<tr style="background-color: #cccccc;">
<td class="tableHeader">Output</td>
</tr>
<tr style="background-color: #eeeeee;">
<td>
<pre class="ng-binding">1
1
1
2
2
3
3
4
4
</pre>
</td>
</tr>
</tbody>
</table>
<!-- end ngRepeat: input in problemDetails.sampleInput track by $index -->
<p><strong>Explanation for sample case</strong></p>
<p>Notation: { swordsman troop number: monster number(s) defeated } { archer troop number: monster number(s) defeated }<br> 1<sup>st</sup> day: {<strong>1</strong>: 1} {}<br> 2<sup>nd</sup> day: {<strong>1</strong>: 1 2} {}<br> 3<sup>rd</sup> day: {<strong>1</strong>: 1 2 3} {}<br> 4<sup>th</sup> day: {<strong>1</strong>: 1 2 3} {<strong>1</strong>: 4}<br> 5<sup>th</sup> day: {<strong>1</strong>: 1 2 3} {<strong>1</strong>: 4 5}<br> 6<sup>th</sup> day: {<strong>1</strong>: 1 2 3; <strong>3</strong>: 6} {<strong>1</strong>: 4 5}<br> 7<sup>th</sup> day: {<strong>1</strong>: 1 2 3; <strong>3</strong>: 6 7} {<strong>1</strong>: 4 5}<br> 8<sup>th</sup> day: {<strong>1</strong>: 1 2 3; <strong>3</strong>: 6 7; <strong>4</strong>: 8} {<strong>1</strong>: 4 5}<br> 9<sup>th</sup> day: {<strong>1</strong>: 1 2 3; <strong>3</strong>: 6 7; <strong>4</strong>: 8 9} {<strong>1</strong>: 4 5}</p>
<p>&nbsp;</p>
<p><strong>Information</strong></p>
<ul>
<li>The constraints above is not typo, N and M can be as large as 1000 (1 Thousand), so H can be as large as 10<sup>6</sup> (1 Million). So this problem has 10¡Á larger constraints than the original one.</li>
<li>Warning: Large Input/Output files, each file I/O can be as large as 7.5 Megabytes (7.5 MB), cin or cout probably too slow for I/O, it's recommended to use scanf/printf (I've tested it).</li>
<li>If you find this problem too hard, you can try this first: <a href="https://jollybeeoj.com/problem/view/199" target="_blank">https://jollybeeoj.com/problem/view/199</a>&nbsp;original problem with smaller constraints.</li>
</ul>
<p>&nbsp;</p>
<p><strong>Trivia</strong></p>
<ul>
<li>The total size of file I/O in this problem is slightly more than 100 MB, took a while to generate, modify, and upload it. :)</li>
<li>If the witch attack Jolly Kingdom everyday for 1 Million days that means the attack took more than 2500 years. :o</li>
<li>If I count number of operation in the deepest loop of my algo on worst case input, it will be 671,163,499 operations.</li>
</ul>
<p>&nbsp;</p>
<p><strong>Credit &amp; Special thanks</strong></p>
<ul>
<li><a title="Sandy Karunia" href="https://id.linkedin.com/in/sandy-karunia-150097a8" target="_blank">Sandy Karunia</a> - Developer of <a href="https://jollybeeoj.com/" target="_blank">Jollybee Online Judge</a></li>
<li><a title="Alvin Setiadi" href="https://id.linkedin.com/in/alvin-setiadi-512289aa" target="_blank">Alvin Setiadi</a> - Original problem author</li>
</ul>
<p>&nbsp;</p>