<p>
Little Ivan likes to play games in his spare time. Unfortunately, he cannot always enjoy the company of his friends and sometimes he is a little bored when he is alone. Therefore, he makes up games, where he is the only player. He is especially proud of his last game and likes to tell you about it. <br>
You are given two finite sequences of positive integers. The game consists of making consecutive moves. You are allowed to make the following move. You remove the last K1 numbers (K1¡Ý1) from the first sequence (possibly the whole sequence) and find their sum S1 and the last K2 numbers (K2¡Ý1) from the second sequence (again you can remove the whole sequence) and find their sum S2. Then you calculate the cost of the move to be (S1 ¨C K1)*(S2 ¨C K2). You continue to make moves until you remove all the numbers in both sequences. The total cost of the game is the sum of the costs of all moves. Your goal is to minimize this total cost. You are not allowed to leave one of the sequences empty, while the other is not. <br>
As Ivan has told you the rules of the game, you realize that it is easily solvable with the help of a computer, so you decide to write a program GAME, that computes the minimum total cost of the game.

</p><h3>Input</h3>
<p> Input data is read from the standard input and consists of three lines. The first line contains two space-separated integers, L1 and L2 (1 ¡Ü L1, L2 ¡Ü 2000), which denote the lengths of the two sequences. The second line contains L1 space-separated integers, which are the elements of the first sequence. The third line contains L2 space-separated integers, which are the elements of the second sequence. The elements of the sequences do not exceed 1000.

</p><h3>Output</h3>
<p>Your program has to output one line on the standard output that contains only one number ¨C the minimum total cost of the game as described above.

</p><h3>Example</h3>

<pre><b>Input:</b>
3 2
1 2 3
1 2
<b>Output:</b>
2
</pre>