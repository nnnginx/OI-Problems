<p>Mathematicians have always loved generalizing mathematics to everything. They even contributed lots of optimizations and valuable formulas to Computer Science. Have you heard about String Multiplication? What do you think will happen if we write the following code in python?</p>
<p><em>print (3 * ¡°abc¡±);</em></p>
<p>As you might have guessed, it prints ¡°abcabcabc¡±. It is equal to <em>print(¡°abc¡± + ¡°abc¡± + ¡°abc¡±);</em></p>
<p>We define string S is divisible by string T, if there is some non-negative integer k, which satisfies the equation S=k*T .</p>
<p>Your task is simple. Given two strings S and T. What is the minimum number of characters which should be removed from S, so S is divisible by T?</p>
<h3>Input</h3>
<p>The first line of the input contains Q the number of the test cases. (1¡ÜQ¡Ü100)</p>
<p>Each test case consists of two lines.&nbsp;</p>
<p>The first line contains string S consisting of lowercase English letters. (0¡Ü|S|¡Ü10<sup>4</sup>)</p>
<p>The second line contains string T consisting of lowercase English letters. (0&lt;|T|¡Ü10<sup>4</sup>)</p>
<h3>Output</h3>
<p>For each test case print a single integer, the minimum number of characters which should be removed.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4
babbaba
ab
dictate
acid

abc
p
q

<strong>Output:</strong>
3
7
0
1
</pre>