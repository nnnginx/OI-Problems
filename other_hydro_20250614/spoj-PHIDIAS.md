<p>
Famous ancient Greek sculptor Phidias is making preparations to build another marvelous
monument. For this purpose he needs rectangular marble plates of sizes W1 x H1, W2 x
H2, ..., WN x HN.<br><br>

Recently, Phidias has received a large rectangular marble slab. He wants to cut the slab to
obtain plates of the desired sizes. Any piece of marble (the slab or the plates cut from it) 

can be cut either horizontally or vertically into two rectangular plates with integral widths 

andheights, cutting completely through that piece. This is the only way to cut pieces and 

piecescannot be joined together. Since the marble has a pattern on it, the plates cannot be 

rotated: if Phidias cuts a plate of size A ? B then it cannot be used as a plate of size B ? A 

unless A = B. He can make zero or more plates of each desired size. A marble plate is wasted if 

it is not of any of the desired sizes after all cuts are completed. Phidias wonders how to cut 

the initial slab so that as little of it as possible will be wasted.<br><br>

As an example, assume that in the figure below the width of the original slab is 21 and the
height of the original slab is 11, and the desired plate sizes are 10 x 4, 6 x 2, 7 x 5, and 15 

x 10. The minimum possible area wasted is 10, and the figure shows one sequence of cuts
with total waste area of size 10.<br></p>
<h3><img src="/content/turbo:PHIDIAS.png"></h3><br>
<p></p>
Your task is to write a program that, given the size of the original slab and the desired plate
sizes, calculates the minimum total area of the original slab that must be wasted.<br>
<p></p>

<h3>Input</h3>
<p>
t - the number of test cases, then t test cases follow [t &lt;= 20]. 

The first line of each test case contains two integers: first W, the width of the original slab, and then H, the height of the original slab. The second line contains one integer N: the number of desired plate sizes. The following N lines contain the desired plate sizes. Each of these lines contains two integers: first the width Wi and then the height Hi of that desired plate size (1 &lt;= i &lt;= N). [1 &lt;= W &lt;= 600, 1 &lt;= H &lt;= 600, 0 &lt; N &lt;= 200, 1 &lt;= Wi &lt;= W, and 1 &lt;= Hi &lt;= H.]<br>
</p>

<h3>Output</h3>
<p>For each test case output one line with a single integer: the minimum total area of the original slab that must be wasted.</p>

<h3>Example</h3>

<pre><b>Input:</b>
1
21 11
4
10 4
6 2
7 5
15 10

<b>Output:</b>
10

</pre>