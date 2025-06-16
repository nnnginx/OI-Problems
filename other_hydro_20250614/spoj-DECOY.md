<p>Apparently, both sides of the battle are now using some sort of cat-and-mouse tactics on the battlefield. The rules are as follows: there are two battles happening simultaneously at different fields. The armies take turns retreating one of their two units to a different location; the retreat of an army automatically causes the opposing army on the same field to follow it. The one that is cornered (that is, has nowhere to retreat on their turn) will be the one that ultimately loses the battle. Given the description of the fields, and supposing that both commanders are perfect strategists, can you decide who is going to win?</p>
<h3>Input</h3>
<p>The first line of input contains an integer <strong>T</strong>, the number of test cases. Each test case consists of two descriptions of the fields of the battle. A description begins with a line containing integers <strong>N </strong>(1 <span>¡Ü</span> N <span>¡Ü</span> 100), <strong>M</strong> (1 <span>¡Ü</span> M <span>¡Ü</span> 10000), the number of locations in the field and the number of roads connecting the locations, respectively. The following <strong>M</strong> lines each contain two integers <strong>u</strong>,<strong>v</strong> (1 <span>¡Ü u,v </span><span>¡Ü N) denoting that there is a one-way road connecting position u to the position v.</span> The initial location of all units is at position 1 in their respective fields.</p>
<h3>Output</h3>
<p>For each test case, output a single line containing the result of the battle, assuming your side is the first to play. Print "I lose" if you're going to lose, "I win" if you're guaranteed to win or "Deadlock" if the battle will go on forever.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3<br>2 1<br>1 2<br>2 1<br>1 2<br>2 2<br>1 2<br>2 1<br>2 1<br>1 2<br>3 2<br>1 2<br>2 3<br>2 1<br>1 2

<strong>Output:</strong>
I lose<br>Deadlock<br>I win <br></pre>