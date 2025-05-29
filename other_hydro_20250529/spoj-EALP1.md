<div style="background-image: initial; background-attachment: initial; background-origin: initial; background-clip: initial; margin: 8px;">
<p>All of must you know the game of Nim. For those who don¡¯t know, I will describe the game in brief:</p>
<p><strong><em>There are two players and there are N piles. Each pile contains some stones. Player 1 takes the first turn, than player 2, than again player 1 and so on. At each turn, the player chooses any ONE pile, and removes at least one stone from it. </em></strong><strong><em>The player who makes the last move wins.</em></strong></p>
<p>Now given N piles, your task is to find the number of ways Player 1 can start the game so that after his first move, he is in the winning position.&nbsp; That means after Player 1 has removed some stones from any ONE pile, he will surely win the game if he plays optimally no matter how well Player 2 plays the game.</p>
<p><strong>Input</strong></p>
<p>Input starts with an integer&nbsp;<strong>T (¡Ü 1000)</strong>, denoting the number of test cases.</p>
<p>Each case starts with an integer&nbsp;<strong>N (1 ¡Ü N ¡Ü 1000)</strong>. The next line contains N integers all less than <strong>1000</strong>. The i<sup>th</sup> integer denotes the number of stones in the i<sup>th</sup> pile.</p>
<p><strong>Output&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong></p>
<p>For each case, print the desired result.&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p>2</p><p>3</p><p>11 15 8</p><p>3</p><p>11 15 7</p><strong>Output:</strong>
<p>Case 1: 3</p><p>Case 2: 3</p></pre>
</div>