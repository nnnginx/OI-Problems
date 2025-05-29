<h3>Background</h3>
<p>Tan always creates some interesting and strange games to kill time,and the Pick-Number Game on Tree is his favorite one.He got the idea from his another game(Pick-Number Game on sequence): there is an integer sequence, he picks a number from the head or the tail of the sequence each turn.When the sequence gets empty,he gets another sequence A,in which A[i] is the <i>i</i>-th integer he picks, then he calculates:</p>
<p>S=A[0]*5<sup>0</sup>+A[1]*5<sup>1</sup>+...+A[n-1]*5<sup>n-1</sup>, while n is the length of the sequence.If S modudo 8 equals to 3,he wins, otherwise he loses(Tan is such a strange person that he likes games with strange rules).</p>
<p>Tan got tired of generating sequence randomly before playing a game, and he changed the rule to avoid it.This time he plays the game on trees. He generates a big tree. Every time he wants to play, he chooses two nodes (A,B) randomly and he finds the path connected A,B (including A,B).In this way he gets a sequence and he can play games.He calls this game "Game(A,B)".He can play many times on a big tree without generating a new one.If he can win in Game(A,B),he says that Game (A,B) is a good game,otherwise Game(A,B) is a bad game.</p>
<p>If a game is a bad game,he can never win,so he has to find a way to identify if a game is bad or good.</p>
<p>He played this game for a long time,and he thought he found a great law: if Game(A,B) is a good game and Game(B,C) is a good game,then Game(A,C) is a good game.And if Game(A,B) is a bad game and Game(B,C) is a bad game,the (A,C) is a bad game.But soon he found it was wrong,but he wanted to know in how many cases it is right.</p>
<p>P.S:"Tan" in Chinese means funny and droll. And Mr.Tan in the story is a real person.</p>
<h3>Task</h3>
<p>The input data describes a tree with integer numbers on each of its nodes.You should count the number of triple (A,B,C) (A,B,C are distinct nodes) that (A,B),(B,C),(A,C) are all good games or all bad games((A,B,C) and (B,C,A) are supposed to be counted once).</p>
<h3>Input</h3>
<p>The first line of the test data is the number of test case t,then t test case follow.</p>
<p>For each test case:</p>
<p>The first line contains a single integer M,the number of nodes in the tree(M&lt;=100000).</p>
<p>M lines follow, each contains two integers F<sub>i</sub> and V<sub>i</sub>. F<sub>i</sub> is the father of node i (F<sub>i</sub>=0 if node i is the root).V<sub>i</sub> is the number on the node i.(0&lt;=V<sub>i</sub>&lt;=40000)</p>
<h3>Output</h3>
<p>For each test case:</p>
<p>The first and only line contains a single integer S, which means there are S triples(A,B,C) that (A,B),(B,C),(A,C) are all good games or all bad games.</p>
<h3>Example</h3>
<pre><b>Input:</b>
1
3
0 3
1 5
1 7

<b>Output:</b>
0
</pre>
<b>Warning: large input/output data, be careful with certain languages</b>