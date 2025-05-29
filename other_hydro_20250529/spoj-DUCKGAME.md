<p><span style="font-size: small;">In a large farm, N ducks are standing and making a big circle. They are numbered 1 to N. Their position are sorted in clockwise and the N<sup>th</sup> duck is adjacent to the first duck.</span></p>
<p><span style="font-size: small;">Then, they will make a game with the following rules :<br></span></p>
<ul>
<li><span style="font-size: small;">the game is played in N rounds</span></li>
</ul>
<ul>
<li><span style="font-size: small;">first round is to decide who is the N<sup>th</sup> winner, </span><span style="font-size: small;">second round is to decide who is the (N-1)<sup>th</sup> winner </span><span style="font-size: small;">and so on until N<sup>th</sup> round is to decide who is the champion (1<sup>st</sup> winner)</span><span style="font-size: small;">. formally, i<sup>th</sup> round is to decide who is the (N-i+1)<sup>th</sup> winner</span></li>
</ul>
<ul>
<li><span style="font-size: small;">in each round i (1 <span style="font-size: small;"><span style="font-size: small;">¡Ü i <span style="font-size: small;"><span style="font-size: small;">¡Ü N)</span></span></span></span>, Mr. Dengklek as a moderator counting the ducks in clockwise direction. </span><span style="font-size: small;">A<sub>i</sub><sup>th</sup> duck will be the winner in this round</span><span style="font-size: small;">, that duck will not play anymore and get out from the circle</span></li>
</ul>
<ul>
<li><span style="font-size: small;">in the first round, Mr. Dengklek starts counting from the first duck. </span><span style="font-size: small;">then in i<sup>th</sup> round (1 &lt; i<span style="font-size: small;"> ¡Ü </span>N), Mr. Dengklek will start counting from the duck after the previous round winner</span></li>
</ul>
<p><span style="font-size: small;">A is an array of N integer with A<sub>1</sub> = L. For 1 &lt; i <span style="font-size: small;">¡Ü </span>N, if A<sub>i-1</sub> = R then A<sub>i </sub>= L. Otherwise, A<sub>i</sub> = A<sub>i-1</sub> + 1.</span></p>
<p><span style="font-size: small;">Because the number of ducks is too large, so the game won't be finished even though in one century. <span style="font-size: small;">Here, you are to find the fastest algorithm to know the M<sup>th</sup> winner (with given N, L, and R) in less than 2 seconds.</span></span></p>
<h3>Input</h3>
<p><span style="font-size: small;">Input contains 2 lines only.</span></p>
<p><span style="font-size: small;">In the first line, given N and M separated by a white space.</span></p>
<p><span style="font-size: small;">The last line contain 2 integers represent L and R.<br></span></p>
<h3>Output</h3>
<p><span style="font-size: small;">The only line contain one number represent the M<sup>th</sup> winner of that game.</span></p>
<h6><span style="font-size: large;">Constraint</span></h6>
<p><span style="font-size: small;">1 <span style="font-size: small;"> ¡Ü M <span style="font-size: small;"> ¡Ü </span></span>N</span><span style="font-size: small;"> ¡Ü 10<sup>18</sup></span></p>
<p><span style="font-size: small;">1 <span style="font-size: small;"> ¡Ü L <span style="font-size: small;"> ¡Ü R <span style="font-size: small;"> ¡Ü 10<sup>18</sup></span></span></span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;"><span style="font-size: small;"><span style="font-size: small;">N-M <span style="font-size: small;"> ¡Ü 10<sup>8</sup> or R <span style="font-size: small;"> ¡Ü 10<sup>5</sup></span></span></span></span></span></span></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5 3
2 4
<strong>Output:</strong>
1</pre>
<h6><span style="font-size: large;">Explanation</span></h6>
<p><span style="font-size: small;"><span style="font-size: small;"><span style="font-size: small;"><span style="font-size: small;"><span style="font-size: small;"><span style="font-size: small;">A = {2,3,4,2,3}</span></span></span></span></span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;"><span style="font-size: small;"><span style="font-size: small;"><span style="font-size: small;"><span style="font-size: small;">round 1 :<br>&nbsp;&nbsp; &nbsp;1 - 2<br>&nbsp;&nbsp; &nbsp;second duck become the 5<sup>th</sup> winner and get out from the game<br>round 2 :<br>&nbsp;&nbsp; &nbsp;3 - 4 - 5<br>&nbsp;&nbsp; &nbsp;start counting from 3<sup>th</sup> duck because the previous winner is the second duck<br>round 3 :<br>&nbsp;&nbsp; &nbsp;1 - 3 - 4 - 1<br>&nbsp;&nbsp; &nbsp;after the last duck is the first duck because they are standing in a circle<br>&nbsp;&nbsp; &nbsp;second duck and 5<sup>th</sup> duck skipped because they are not playing anymore<br>round 4 :<br>&nbsp;&nbsp; &nbsp;3 - 4<br>&nbsp;&nbsp; &nbsp;A<sub>4</sub> = L = 2 because A<sub>3</sub> = 4 = R<br>round 5 :<br>&nbsp;&nbsp; &nbsp;3 - 3 - 3<br>&nbsp;&nbsp; &nbsp;3<sup>th</sup> duck is the champion</span></span></span></span></span></span></p>
<p>&nbsp;</p>