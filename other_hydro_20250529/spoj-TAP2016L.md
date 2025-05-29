<p><strong>Due to SPOJ restrictions, this problem has been modified with respect to the original version used in the Argentinian Programming Tournament of 2016 in order to have multiple test cases per input file. The original version of this problem (in Spanish) can be found at <a href="http://torneoprogramacion.com.ar/wp-content/uploads/2016/09/tap2016.pdf">http://torneoprogramacion.com.ar/wp-content/uploads/2016/09/tap2016.pdf</a> ]</strong></p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><strong>Leonardo de Pisa is a very cautious man, and even though Christmas is still many months away, he has already bought his Christmas tree. It is a very, very high tree, even higher than the Tower of Pisa. Leonardo wishes to decorate his tree by using colored balls and lights. To that end, he has bought many balls of each possible integer diameter between 1 and N. In fact, he has bought so many balls that he has no idea of what to do with all of them.</strong></div>
<p><strong> </strong></p>
<p><strong> </strong></p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">In Pisa, each ball has two cords hanging from it, to which other balls can be attached. By doing so, they make sure that the balls never fall from the tree and roll all the way across the floor, until finally stopping underneath a big piece of furniture where they cannot easily be found. All of the cords hanging from all of the balls have a length of 20 centimeters.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Just like any good Christmas tree, Leonardo's tree has a top. On it, Leonardo will place a ball of diameter N, as those are the most alluring. All of the other balls in the tree will hang from this top ball either directly, or indirectly by means of other balls. Leonardo has carefully studied the way in which he must hang the balls so that his tree is the most beautiful tree in all of Pisa, and he has arrived at the following conclusions:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; * No ball of diameter 1 or 2 must have another ball hanging from it.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; * Every ball of diameter k &gt;= 3 must have two balls hanging from it: one of diameter k-1, and the other of diameter k-2.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp;&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The following pictures show two examples of how Leonardo's tree would look after decorating it with balls. The left figure corresponds to the case in which he buys every ball up to diameter N = 4, while the right figure corresponds to the case with balls of diameter up to N = 5 (the number written on each ball indicates its diameter).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&lt;PICTURES&gt;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">There is always enough room for Leonardo to add as many balls as he wants, for his tree is incredibly tall. However, he still feels that his tree is not the most beautiful tree in the city: It is missing colored lights!</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Leonardo has bought a special string of lights suitable for trees with balls. The string has K lights tied together by cord, such that the lights are separated from each other by 20 centimeters of cord. Each light fits perfectly onto some balls, depending solely on their size: a light of type i only fits onto balls of diameter i, for each i between 1 and N. If the diameter of the ball is larger than i, the ball will not fit, and if it is smaller than i, the light will fall to the floor. Two lights can never be attached to the same ball, and the cord between the lights must always be perfectly tight. In particular, that means that if there is no cord in the tree between two balls, then their distance will not be exactly 20 centimeters, and so it will not be possible to place two consecutive lights on top of them.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The following picture shows four different strings of lights, colored gray.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&lt;PICTURES&gt;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">By the time that Leonardo bought the string of lights, he had already finished decorating his tree with balls. It was such an effort to do so, that he is completely determined not to add, remove, or move any ball from the tree. Now he does not know if he will be able to use the string of lights that he bought, as he needs to find a sequence of balls in the tree that are adequately hanging from each other, and that have precisely the diameters that the lights fit onto.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">For example, the first string previously shown can be placed on each of the two trees; the second one can only be placed in the second tree; the third and fourth strings cannot be placed on any tree. The following picture shows the first string placed on the first tree, and the second string placed on the second tree.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&lt;PICTURES&gt;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Help Leonardo to know, given the string of lights and the diameter N of the largest ball that he bought, whether it is possible to place the string of lights on his tree</div>
<p>Leonardo de Pisa is a very cautious man, and even though Christmas is still many months away, he has already bought his Christmas tree. It is a very, very high tree, even higher than the Tower of Pisa. Leonardo wishes to decorate his tree by using colored balls and lights. To that end, he has bought many balls of each possible integer diameter between <strong>1</strong> and <strong>N</strong>. In fact, he has bought so many balls that he has no idea of what to do with all of them.</p>
<p>In Pisa, each ball has two cords hanging from it, to which other balls can be attached. By doing so, they make sure that the balls never fall from the tree and roll all the way across the floor, until finally stopping underneath a big piece of furniture where they cannot easily be found. All of the cords hanging from all of the balls have a length of 20 centimeters.</p>
<p>Just like any good Christmas tree, Leonardo's tree has a top. On it, Leonardo will place a ball of diameter <strong>N</strong>, as those are the most alluring. All of the other balls in the tree will hang from this top ball either directly, or indirectly by means of other balls. Leonardo has carefully studied the way in which he must hang the balls so that his tree is the most beautiful tree in all of Pisa, and he has arrived at the following conclusions:</p>
<ul>
<li>No ball of diameter <strong>1</strong> or <strong>2</strong> must have another ball hanging from it.</li>
<li>Every ball of diameter <strong>k ¡Ý&nbsp;3</strong> must have two balls hanging from it: one of diameter <strong>k-1</strong>, and the other of diameter <strong>k-2</strong>.</li>
</ul>
<p>The following pictures show two examples of how Leonardo's tree would look after decorating it with balls. The left figure corresponds to the case in which he buys every ball up to diameter <strong>N = 4</strong>, while the right figure corresponds to the case with balls of diameter up to <strong>N = 5</strong> (the number written on each ball indicates its diameter).</p>
<p style="text-align: center;"><img src="../../content/fidels:TAP2016L1.png" alt=""></p>
<p>There is always enough room for Leonardo to add as many balls as he wants, for his tree is incredibly tall. However, he still feels that his tree is not the most beautiful tree in the city: It is missing colored lights!</p>
<p>Leonardo has bought a special string of lights suitable for trees with balls. The string has <strong>K</strong> lights tied together by cord, such that the lights are separated from each other by 20 centimeters of cord. Each light fits perfectly onto some balls, depending solely on their size: a light of type <strong>i</strong> only fits onto balls of diameter <strong>i</strong>, for each <strong>i</strong> between <strong>1</strong> and <strong>N</strong>. If the diameter of the ball is larger than <strong>i</strong>, the ball will not fit, and if it is smaller than <strong>i</strong>, the light will fall to the floor. Two lights can never be attached to the same ball, and the cord between the lights must always be perfectly tight. In particular, that means that if there is no cord in the tree between two balls, then their distance will not be exactly 20 centimeters, and so it will not be possible to place two consecutive lights on top of them.</p>
<p>The following picture shows four different strings of lights, colored gray.</p>
<p style="text-align: center;"><img src="../../content/fidels:TAP2016L2.png" alt=""></p>
<p>By the time that Leonardo bought the string of lights, he had already finished decorating his tree with balls. It was such an effort to do so, that he is completely determined not to add, remove, or move any ball from the tree. Now he does not know if he will be able to use the string of lights that he bought, as he needs to find a sequence of balls in the tree that are adequately hanging from each other, and that have precisely the diameters that the lights fit onto.</p>
<p>For example, the first string previously shown can be placed on each of the two trees; the second one can only be placed in the second tree; the third and fourth strings cannot be placed on any tree. The following picture shows the first string placed on the first tree, and the second string placed on the second tree.</p>
<p style="text-align: center;"><img src="../../content/fidels:TAP2016L3.png" alt=""></p>
<p>Help Leonardo to know, given the string of lights and the diameter <strong>N</strong> of the largest ball that he bought, whether it is possible to place the string of lights on his tree.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>There are multiple test cases in the input file. For each test case, the first line contains two integers <strong>N</strong> and <strong>K</strong>, with <strong>N</strong> representing the maximum diameter of the balls, and <strong>K</strong> representing the number of lights in the string (<strong>2 ¡Ü&nbsp;N, K&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;10<sup>5</sup></strong>). The second line contains <strong>K</strong> integers <strong>L<sub>1</sub>, L<sub>2</sub>, ..., L<sub>k</sub></strong> describing the string of lights. The ith integer <strong>L<sub>i</sub></strong> represents the type of the <strong>i-</strong>th light in the string (<strong>1&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;L<sub>i</sub>&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;N</strong> for <strong>i</strong> between <strong>1</strong> and <strong>K</strong>).</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case, write a single line containing a single character, indicating whether Leonardo can place the string of lights or not. The character must be an '<strong><span style="font-family: &quot;courier new&quot;, courier;">S</span></strong>' if Leonardo can place the string of lights, and an '<strong><span style="font-family: &quot;courier new&quot;, courier;">N</span></strong>' otherwise.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-family: &quot;courier new&quot;, courier;">3 2
2 3
4 4
1 3 4 2
5 2
3 5
4 2
4 1
6 3
2 3 2
8 4
2 3 3 1
10 10
2 3 4 5 6 8 7 5 3 1</span>

<strong>Output:</strong>
<span style="font-family: &quot;courier new&quot;, courier;">S
S
S
N
N
N
S</span><span style="white-space: normal;">
</span></pre>