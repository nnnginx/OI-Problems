<p>Arya and Bran are playing a game. Initially, two positive integers&nbsp;<strong>A</strong>&nbsp;and&nbsp;<strong>B</strong>&nbsp;are written on a blackboard. The players take turns, starting with Arya. On his or her turn, a player can replace&nbsp;<strong>A</strong>&nbsp;with&nbsp;<strong>A</strong>&nbsp;-&nbsp;<strong>k</strong>*<strong>B</strong>&nbsp;for any positive integer&nbsp;<strong>k</strong>, or replace&nbsp;<strong>B</strong>&nbsp;with&nbsp;<strong>B</strong>&nbsp;-&nbsp;<strong>k</strong>*<strong>A</strong>&nbsp;for any positive integer&nbsp;<strong>k</strong>. The first person to make one of the numbers drop to zero or below loses.</p>
<p>For example, if the numbers are initially (12, 51), the game might progress as follows:</p>
<ul>
<li style="margin-bottom: 0.25em;">Arya replaces 51 with 51 - 3*12 = 15, leaving (12, 15) on the blackboard.</li>
<li style="margin-bottom: 0.25em;">Bran replaces 15 with 15 - 1*12 = 3, leaving (12, 3) on the blackboard.</li>
<li style="margin-bottom: 0.25em;">Arya replaces 12 with 12 - 3*3 = 3, leaving (3, 3) on the blackboard.</li>
<li style="margin-bottom: 0.25em;">Bran replaces one 3 with 3 - 1*3 = 0, and loses.</li>
</ul>
<p>We will say (<strong>A</strong>,&nbsp;<strong>B</strong>) is a&nbsp;<em>winning</em>&nbsp;position if Arya can always win a game that starts with (<strong>A</strong>,<strong>B</strong>) on the blackboard, no matter what Bran does.</p>
<p>&nbsp;</p>
<p>Given four integers&nbsp;<strong>A<sub>1</sub></strong>,&nbsp;<strong>A<sub>2</sub></strong>,&nbsp;<strong>B<sub>1</sub></strong>,&nbsp;<strong>B<sub>2</sub></strong>, count how many winning positions (<strong>A</strong>,&nbsp;<strong>B</strong>) there are with&nbsp;<strong>A<sub>1</sub></strong>&nbsp;¡Ü&nbsp;<strong>A</strong>&nbsp;¡Ü&nbsp;<strong>A<sub>2</sub></strong>&nbsp;and&nbsp;<strong>B<sub>1</sub></strong>&nbsp;¡Ü&nbsp;<strong>B</strong>&nbsp;¡Ü&nbsp;<strong>B<sub>2</sub></strong>.</p>
<h3>Input</h3>
<p>The first line of the input gives the number of test cases,&nbsp;<strong>T</strong>.&nbsp;<strong>T</strong>&nbsp;test cases follow, one per line. Each line contains the four integers&nbsp;<strong>A<sub>1</sub></strong>,&nbsp;<strong>A<sub>2</sub></strong>,&nbsp;<strong>B<sub>1</sub></strong>,&nbsp;<strong>B<sub>2</sub></strong>, separated by spaces.</p>
<p>1 ¡Ü&nbsp;<strong>T</strong>&nbsp;¡Ü 250.&nbsp;<br>1 ¡Ü&nbsp;<strong>A<sub>1</sub></strong>&nbsp;¡Ü&nbsp;<strong>A<sub>2</sub></strong>&nbsp;¡Ü 1,000,000.<br>1 ¡Ü&nbsp;<strong>B<sub>1</sub></strong>&nbsp;¡Ü&nbsp;<strong>B<sub>2</sub></strong>&nbsp;¡Ü 1,000,000.<br><strong>A<sub>2</sub></strong>&nbsp;-&nbsp;<strong>A<sub>1</sub></strong>&nbsp;¡Ü 999,999.<br><strong>B<sub>2</sub></strong>&nbsp;-&nbsp;<strong>B<sub>1</sub></strong>&nbsp;¡Ü 999,999.</p>
<h3>Output</h3>
<p>For each test case, output one line containing "Case #x: y", where x is the case number (starting from 1), and y is the number of winning positions (<strong>A</strong>,&nbsp;<strong>B</strong>) with&nbsp;<strong>A<sub>1</sub></strong>&nbsp;¡Ü&nbsp;<strong>A</strong>&nbsp;¡Ü&nbsp;<strong>A<sub>2</sub></strong>&nbsp;and&nbsp;<strong>B<sub>1</sub></strong>¡Ü&nbsp;<strong>B</strong>&nbsp;¡Ü&nbsp;<strong>B<sub>2</sub></strong>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3<br>5 5 8 8<br>11 11 2 2<br>1 6 1 6

<strong>Output:</strong>
<code style="color: black; font-family: 'bogus font here', monospace; font-size: 13px;">Case #1: 0<br>Case #2: 1<br>Case #3: 20<br><br></code></pre>