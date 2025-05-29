<p>Marcos the little one decided to build and manage an espionage agency, he was happy working as the chief of his agency, hiring spies to spy everybody in the country! But he realized that some of their own spies are spying themselves, of course, this is bad to the business and he don't want this to happen, he wants a program to alert him whenever a spy is spying another spy.</p>

<h3>Input</h3>
<p>Will consists in T test cases, then, T cases will follow, starting from two integers N and R, each one denoting the number of persons to evaluate and the number of relationships spy-person each one has, then, R lines will follow and will contain two integers R1 and R2, meaning that R1 spies R2.</p>

<h3>Output</h3>
<p>Will consist in T lines, starting from the string ¡°<tt>Scenario #i: </tt>¡° where i is the number of the test case you're analyzing, print the string ¡°<tt>spying</tt>¡± if each spy has as a target a civilian, print ¡°<tt>spied</tt>¡± otherwise.</p>

<p><strong>Input</strong></p>
<pre>3
3 2
0 1
2 1
3 3
0 1
2 1
0 2
4 2
2 3
0 1</pre>

<p><strong>Output</strong></p>
<pre>Scenario #1: spying
Scenario #2: spied
Scenario #3: spying</pre>

<h3>Constraints</h3>
<p>1 &lt;= N &lt;= 1000</p>
<p>1 &lt;= R &lt;= 10000</p>

<p><b>Explanation of the second test case:</b></p>
<p>Spy 0 spies civilian 1, spy 2 spies civilian 1, spy 0 spies spy 2. (Spied case).</p>