<p>The mad scientist Byteasar would like to give birth to a new kind of creatures. For this, he has decided to modify the genome of a Bytean mouse.</p>
<p>A DNA can be described as a sequence nucleotides denoted by letters A, C, G and T. Byteasar¡¯s master plan is quite simple: using the DNA of a mouse, he is going to create a new DNA of the same length that is as little similar to the mouse¡¯s DNA as possible. The similarity of two DNAs is the length of their longest common subsequence. The longest common subsequence of two words x, y is defined as the longest word that can be obtained from each of x, y by removing some (possibly none) letters from both words. (Note that two words may have several longest common subsequences. For example, the longest common subsequences of the words CACCA and CAAC are: CAA and CAC.) Write a program that computes the requested DNA.</p>
<h3>Input</h3>
<p>The first line of input contains one integer n (1 ¡Ü n ¡Ü 10000), the length of the DNA of a Bytean mouse. The second line contains a description of nucleotides in the DNA: a sequence of n uppercase letters A, C, G, T.</p>
<h3>Output</h3>
<p>The first line of output should contain one integer: the similarity of the Bytean mouse's DNA and the DNA computed by your program. The second line should hold a sequence of letters A, C, G, T. This should be a DNA that is as little similar to the DNA from the input as possible. Should there be many correct answers, your program may output any one of them.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4
GACT

<strong>Output:</strong>
1
TCAG
</pre>