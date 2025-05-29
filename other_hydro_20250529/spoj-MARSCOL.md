<p>Martian Colony is one of the best single player strategy games developed by a renowned game development company. The player has to destroy several colonies on Mars while playing the game.</p>
<p>The planet Mars has <strong>N</strong> villages numbered from <strong>1</strong> to <strong>N</strong>. Among the villages, the village numbered <strong>i</strong> has <strong>di</strong> amount of Diamonds. There are <strong>E</strong> one-way roads between some pair of villages, that is, if there is a road from village <strong>u</strong> to village <strong>v</strong>, Martians can only move from village <strong>u</strong> to village <strong>v</strong>. A number of villages make a colony when for every pair of villages <strong>u</strong> and <strong>v</strong> of that colony, there is a path from village <strong>u</strong> to the village <strong>v</strong> and the opposite. A path is a sequence of several roads. Each colony has some hit points which is the sum of the lengths of the roads inside that colony. A colony can be destroyed by using marsa points equal to the hit points of that colony. Destroying a colony will add the total number of diamonds of the villages of that colony to the player¡¯s score.</p>
<p>Alon is your best friend. He loves to play strategy games and trying this new one. He loves to score the maximum always. At some stage of the game he is stuck with <strong>M</strong> amount of marsa points. He wonders, what is the highest score he can gain using maximum <strong>M</strong> marsa points. As a best friend of Alon, he seeks your help to calculate the exact score.</p>
<h3>Input</h3>
<p>The first line of input will contain <strong>T</strong> denoting the number of test cases. Before every test case there will be a blank line. The first line of the test cases will contain 3 integers <strong>N, E</strong> and <strong>M ( 1 ¡Ü N ¡Ü 100, 0 ¡Ü E ¡Ü N^2, 1 ¡Ü M ¡Ü 5000 )</strong>. The next line will contain <strong>N</strong> integers <strong>di ( -100 ¡Ü di ¡Ü 100)</strong> that represent the number of diamonds in the ith village. Each of the next E lines will contain three integers <strong>u</strong>, <strong>v</strong> and <strong>w</strong> <strong>( 1 ¡Ü u, v ¡Ü N, 1 ¡Ü w ¡Ü 1000 )</strong> which means there is a road from village <strong>u</strong> to village <strong>v</strong> of length <strong>w</strong>.</p>
<h3>Output</h3>
<p>For each test case print a single line containing <strong>¡°Case X: S¡±</strong>, where X is the case number and <strong>S</strong> is the maximum score Alon can score.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1

3 3 3
3 3 3
1 2 3
2 3 3
2 1 3

<strong>Output:</strong>
Case 1: 3
</pre>