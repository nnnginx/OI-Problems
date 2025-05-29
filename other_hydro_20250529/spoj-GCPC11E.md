<p>One of the recent hypes in terms of independent games has been Minecraft, a cute little game in which you mine some materials and are able to craft a lot of stuff using these materials. Since you already mastered the Minecraft universe, you decide to write your own little mod for the game to add magical crafting.</p>
<p>Given some magic stone <em>m<sub>1</sub></em>, by adding a specific amount of diamonds you can transform it into two magic stones <em>m<sub>2</sub></em> and <em>m<sub>3</sub></em>, where <em>m<sub>1</sub></em>, <em>m<sub>2</sub></em> and <em>m<sub>3</sub></em> are upper-case letters. This is called a crafting recipe.</p>
<p>There is also a default transformation which transforms a magic stone into its matching lighting effect; the matching lighting effect for a magic stone labelled with an upper-case letter is the corresponding lower-case letter, e. g. the magic stone 'A' can be transformed into the lighting effect 'a'. This transformation always costs exactly <em>1</em> diamond. The default transformation is used whenever you do not use a magic stone for another crafting recipe. The lighting effects will show in a certain order. For each used crafting recipe <em>m<sub>1</sub></em> -&gt; <em>m<sub>2</sub></em> <em>m<sub>3</sub></em>, the lighting effects which are derived from the magic stone <em>m<sub>2</sub></em> will show before the lighting effects derived from the magic stone <em>m<sub>3</sub></em>.</p>
<p>You want to be able to craft wonderful magic lights for your own world.  But as you are aware of the rareness of the precious diamonds, and also very picky about the lighting effect sequences you want to achieve, you have to test your crafting recipes. The question arises if your set of crafting recipes allows you to create all your desired lighting effect sequences if you only have the magic stone 'A' to start with, and the minimum number of diamonds you will need for the transformations.</p>
<h3>Input</h3>
<p>The first line of the input gives the number of test cases <em>C</em> (<em>0 &lt; C �� 100</em>). Each test case starts with two integers <em>0 �� R �� 30</em>, <em>0 �� L �� 10</em> on a single line, denoting the set of recipes and the number of lighting effect sequences. The next <em>R</em> lines contain the set of recipes. Each crafting recipe is given on a single line by the magic stones <em>m<sub>1</sub></em>, <em>m<sub>2</sub></em>, and <em>m<sub>3</sub></em> as well as the number <em>d</em> (<em>0 �� d �� 1000</em>) of diamonds necessary for the transformation. The next <em>L</em> lines contain the lighting effect sequences you want to create. Each of these lines contains an integer <em>l</em> (<em>1 �� l �� 100</em>), which represents the length of the lighting effect sequence. The line completes with a single string of length <em>l</em>, consisting only of lower case characters 'a' to 'z', which represents the sequence of lighting effects you want to create.</p>
<h3>Output</h3>
<p>For every test case print <strong>CASE #</strong> followed by the number of the test case, starting with <em>1</em>, on a single line. For each lighting effect sequence print a single line. If the effect is possible print <strong>POSSIBLE WITH </strong><em>X</em><strong> DIAMONDS</strong>, with <em>X</em> representing the number of diamonds you will need to achieve the lighting effect sequence. In the case the lighting effect sequence cannot be crafted, print <strong>IMPOSSIBLE</strong>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
1 4
A A A 2
3 aaa
8 aaaaaaaa
5 ababa
1 a
3 1
A B C 1
C P C 7
B I C 11
4 icpc

<strong>Output:</strong>
CASE #1
POSSIBLE WITH 7 DIAMONDS
POSSIBLE WITH 22 DIAMONDS
IMPOSSIBLE
POSSIBLE WITH 1 DIAMONDS
CASE #2
POSSIBLE WITH 23 DIAMONDS
</pre>