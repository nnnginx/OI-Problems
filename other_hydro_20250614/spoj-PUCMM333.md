<p>
Xorland is a beautiful Kingdom located in the northern part of the Hispaniola Island. You can picture it as a perfect n x n square. Incredibly, n^2 people live there, each in a perfect 1x1 square. They all have an integer spirit in the range [1, 10^6]. The King died recently and, as is custom, Xorland must be divided into three parts.
</p>
<p>
Xorlandic people love to apply the Xor operation on their spirits, so it is normal to expect them to use it also to divide the land. Xorland must be divided by two parallel lines. These parallel lines must also be parallel to one side of the square. Each part will be non-empty. To divide the land, this is what they do:
</p>
<p>(1) Place two parallel lines inside the square.</p>
<p>(2) Construct a non-empty subset of the spirits of the first part and call it A.</p>
<p>(3) Construct a non-empty subset of the spirits of the second part and call it B.</p>
<p>(4) Construct a non-empty subset of the spirits of the third part and call it C.</p>
<p>(4) Apply the Xor operation on A, on B and on C.</p>
<p>(5) Find the value of Xor(A) + Xor(B) + Xor(C) and call it SUM.</p>
<p>(6) Eat and Drink joyfully for SUM days straight.</p>

<p>Between us, Xorlandic people LOVE eating and drinking! That is why they want to find the partition that yields the greatest sum. Help them! Write a program that finds this number.</p>

<h3>Input</h3>
<p>The first line of input contains N (3 &lt;= N &lt;= 5), the length of the sides of the squared area. Then follow N lines, each bearing a spirit. Each spirit will be a positive integer in the range [1, 10^6]. </p>

<h3>Output</h3>
<p>Output the greatest sum possible.</p>

<h3>Sample Cases</h3>
<pre><b>Input</b>
3
1 1 1
2 2 2
3 3 3

<b>Output</b>
9</pre>

<p>In this case, the optimal choice is to divide vertically. Column 1 is {1, 2, 3}; Column 2 is {1, 2, 3} and Column 3 is {1, 2, 3}. Taking A = {3}, B = {3} and C{3} we get 3 * Xor{3} = 9, the optimal answer. Note that other subsets may yield 9 as well. </p>