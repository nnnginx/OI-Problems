<p>Just as promised, PolyProg will invite you to a bounteous pancake buffet right after this contest. Can you already feel the seductive odours dazing your senses? Well, before your mouth starts watering, you should solve this last problem.</p>

<p>
</p><div align="center"><img src="./23770/file/es7seHyK.png" alt="" width="440" height="400"></div>
<p></p>
<p>As you might know, the basic ingredients to pancakes are flour, milk and eggs. These may be completed by a passel of additional toppings such as sugar, jam, berries, cheese, ham, mushrooms etc. As the chef of the evening was yet uncertain about the recipe he¡¯d whip up tonight, he asked his assistant simply to buy random quantities of each ingredient.</p>

<p>With these quantities he could make <em>N1</em> pancakes according to recipe 1, <em>N2</em> if he decides to follow recipe 2, <em>N3</em> for recipe 3 and so on and so forth. As the end of the competition is close, the chef will not have enough time to combine several recipes: All pancakes tonight will be of the same taste (too bad :( ). The repertoire of recipes is huge, and as we imagine you to have a ravenous appetite, you are to select the recipe that yields the largest number of pancakes.</p>

<h3>Input</h3>
<p>The input consists of several test-cases separated by an empty line. The first line of each test-case holds the number of ingredients <em>N (1&lt;=N&lt;=50)</em> the assistant bought followed by the number of recipes <em>R (1&lt;=R&lt;=100) </em>in the chef¡¯s repertoire. Each of the next lines contains exactly <em>N</em> non-negative integers (no larger than 10<sup>6</sup>) informing about the ingredients. The first of these lines lists the quantities the assistant bought of each ingredient. The remaining <em>R</em> lines list the quantities (in the same order as the previous line) necessary to make ten pancakes according to the recipe r<sub>i</sub> (from 1 to <em>R</em>). The input ends on a test-case having both <em>N</em> and <em>R</em> zero, which must not be processed.</p>

<h3>Output</h3>
<p>Your program should produce one line per test-case containing the recipe that yields the largest number of pancakes followed by the number of entire pancakes that can be made then. If there is a tie, prefer the recipe that appears first in the input.</p>

<h4>SAMPLE INPUT</h4>
<pre>3 2
20 20 20
5 10 1
2 1 3
&nbsp;
6 3
100 60&nbsp;130 80&nbsp;100 90
10 5 10 5 10 5
1 2 1 2 20 7
0 0 0 10 30 1
&nbsp;
0 0</pre>

<h4>SAMPLE OUTPUT</h4>
<pre>2 66
1 100
</pre>