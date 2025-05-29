<h3>Background</h3>

<p>Poor You-Know-Who was out of business for quite some time,
being neither dead, nor alive. He would like to get rich so that
he can run for the post of Minister of Magic. From there he could
unfold at least some of his evil plots even if he lost most of
his magical powers. You are fed up with all this Harry Potter
business and decide to help You-Know-Who make some
dough. You-Know-Who inherited lots of magic powder that increases
one's sense of smell for a short period of time if inhaled. He
will sell it and you'll help him maximize the profit.
</p>

<h3>Problem</h3>

<p>You-Know-Who has <tt>C</tt> clients. Client <tt>i</tt> will
buy <tt>a[i]−b[i]*p</tt> powder if the unit price
is <tt>p</tt>. That is, if You-Know-Who shows a certificate
issued by the Minister saying that the asked price is the correct
price. Getting one such certificate involves paying a bribe
<tt>B</tt>. To maximize the profit he may buy several such
certificates and use for each client the one that maximizes his
profit. You must tell You-Know-Who what certificates he should
get. With some luck, Harry Potter is out!
</p>

<h3>Input</h3>
<p>The first line contains the number of testcases, which shall
be less than 20. The testcases follow. (Possible empty lines
between testcases should be ignored.)
</p>

<p>The first line of each testcase input contains two
non-negative integers: the bribe <tt>B</tt> and the number of
clients <tt>C</tt>. The next <tt>C</tt> lines describe each
client by two positive integers <tt>a[i]</tt> and <tt>b[i]</tt>
(on line <tt>i</tt>). You are guaranteed that all numbers in the
input are at most 2000.</p>

<h3>Output</h3>
<p>For each testcase the output is a single
number, the maximum profit of You-Know-Who, and it should be
written on a line by itself. The answer should have either an
absolute or a relative error less than 1e-6.</p>

<h3>Example</h3>

<pre><b>Input:</b>
2
10 2
10 1
20 3
100 1
5 1

<b>Output:</b>
46.25
0
</pre>

<p>First testcase: If YKW would have only the first client then
he should choose to get a certificate for the price 5. This way
he will sell 5 grams of powder for a profit of 5x5-10=15.
Analogously, for the second client the optimal price would be
3.(3), which would make the client buy 10 grams of magic
powder. Choosing the optimal price for each client means that two
bribes must be payed, which leads to a profit of
5x5+10x3.(3)-2x10=38.(3). Nevertheless, YKW can win more money by
getting only one certificate for the price 3.75.  This way the
profit is 6.25x3.75+8.75x3.75-10=46.25.</p>

<p>The second testcase shows that sometimes it's better to
not sell magic powder to some clients.</p>