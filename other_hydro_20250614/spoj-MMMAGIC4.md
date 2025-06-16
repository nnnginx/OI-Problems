<p style="text-align: center;"><img src="../../content/miodziu:disney2.jpg" alt=""></p>
<h3>MMMAGIC4</h3>
<p>Mickey Mouse and Donald Duck love magic. They spacialize with card tricks. Mickey invented a new trick and they are going to surprise the world. They've contracted series of shows on whole the globe, worth many milion of dolars $$. The first show is coming up but unfortunately Mickey lost secret of the trick. He remembers only trick description, but it's not enough to satisfy the contract conditions. Help them!</p>
<h3>Trick description</h3>
<p>Mickey has n cards with values 1, 2, ..., n. He invites a spectator from the audience, Donald is outside the stage and see nothing on the stage. The spectator chooses randomly k cards from the pack and discard the remaining n-k cards. Mickey chooses one card from this k cards, shows it to everyone (except Donald) and hides it to the spectator's pocket. Next Mickey leaves the remaining k-1 cards in some order on the table. Donald is coming back. He is the only person, who don't know, what is the number in the hiden card. He can see only k-1 cards on the table. Donald thinks for a while, the drum rumbles, at the begining very silent, then lauter and lauter,&nbsp;everyone is waiting, the drum stops, a few seconds of deep silence and... Donald says the number on the hidden card. It's correct, applause! How did he discover the number? It's magic!</p>
<h3>Help request</h3>
<p>Mickey and Donald know, that's not magic only smart math manipulations. They asked You to help them. You have to write computer program, that can help them with the trick. The program should be able to do two things: help Mickey to select one card from given k cards and describe order of remaining k-1 cards on the table, then help Donald to guess the hidden card value basing only on k-1 cards left by Mickey on the table. You can use any strategy that You want, but remember - Donald needs to guess the number during the show, because the huge profit $$ depends on it.</p>
<h3>Input</h3>
<p>All integers in the same line are single-space separated (the same concerns problem output).</p>
<p>Values n, k are constant. In this problem n=27 and k=4. There are also problems with different values: <a href="../../problems/MMMAGIC3/">MMMAGIC3</a>, <a href="../../problems/MMMAGIC5/">MMMAGIC5</a>, <a href="../../problems/MMMAGIC6/">MMMAGIC6</a></p>
<p>The first line of input contains two integers M, D, where M is the number of test cases in which Mickey needs help, D is the number of test cases in which Donald needs help (M+D &lt; 40000).</p>
<p>Every of next M lines contains k distinct integers from range [1, n] - the values on cards given to Mickey. The order of values is casual.</p>
<p>Every of next D lines contains k-1 distinct integers from range [1, n] - the cards left to Donald on the table. The order is the same, as on the table, from left to right.</p>
<h3>Output</h3>
<p>For each Mickey's query write a line with k-1 integers - the values on the cards, that Mickey have to leave on the table, from left to right.</p>
<p>For each Donald's query write a line with one integer - the value of hidden card or (if in Your strategy such situation is impossible) any of remaining values.</p>
<h3>Example</h3>
<table border="1">
<tbody>
<tr>
<td>Input 1</td>
<td>Output 1</td>
</tr>
<tr>
<td>3 0<br>1 2 3 4<br>4 13 6 2<br>8 20 7 4</td>
<td><br>3 2 1<br>13 4 6<br>4 20 7</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<table border="1">
<tbody>
<tr>
<td>Input 2</td>
<td>Output 2</td>
</tr>
<tr>
<td>0 3<br>3 2 1<br>13 4 6<br>4 20 7</td>
<td><br>4<br>2<br>8</td>
</tr>
</tbody>
</table>
<h3>Explanation</h3>
<p>The example above don't show any concrete strategy. It just shows, that strategy must be coherent (when Mickey for given set of cards 1 2 3 4 leave on the table 3 2 1, then Donald for given cards 3 2 1 should answer with the number 4).</p>
<p>Generally You can implement Your own strategy satisfying the conditions below:</p>
<ul>
<li>for Mickey's query "a<sub>1</sub> a<sub>2</sub> ... a<sub>k</sub>" You should reply "b<sub>1</sub> b<sub>2</sub> ... b<sub>k-1</sub>", such that {b<sub>1</sub>, b<sub>2</sub>, ..., b<sub>k-1</sub>} is subset of {a<sub>1</sub>, a<sub>2</sub>, ..., a<sub>k</sub>}</li>
<li>for Donald's query "b<sub>1</sub> b<sub>2</sub> ... b<sub>k-1</sub>" reply the number c, such that {b<sub>1</sub>, b<sub>2</sub>, ..., b<sub>k-1</sub>, c} = {a<sub>1</sub>, a<sub>2</sub>, ..., a<sub>k</sub>}</li>
</ul>
<p>&nbsp;</p>
<h3>Note</h3>
<p>The similar problems appeared in MWPZ 2007 contest in Poland, with different story (in original problems there was Polish characters Bolek, Lolek and Jacek, Placek). The main page of contest is <a href="http://mwpz.poznan.pl">http://mwpz.poznan.pl</a></p>