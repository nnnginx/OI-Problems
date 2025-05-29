<p align="justify">
Before ACM can do anything, a&nbsp;budget must be prepared and the necessary
financial support obtained. The main income for this action comes from
Irreversibly Bound Money (IBM). The idea behind is simple. Whenever
some ACM member has any small money, he takes all the coins and throws them
into a piggy-bank. You know that this process is irreversible, the coins
cannot be removed without breaking the pig. After a sufficiently long
time, there should be enough cash in the piggy-bank to pay everything that
needs to be paid.

</p><p align="justify">
But there is a big problem with piggy-banks. It is not possible to
determine how much money is inside. So we might break the pig into
pieces only to find out that there is not enough money.  Clearly, we want to
avoid this unpleasant situation. The only possibility is to weigh the
piggy-bank and try to guess how many coins are inside. Assume that we
are able to determine the weight of the pig exactly and that we know
the weights of all coins of a given currency. Then there is some
minimum amount of money in the piggy-bank that we can guarantee. Your task
is to find out this worst case and determine the minimum amount of
cash inside the piggy-bank. We need your help. No more prematurely
broken pigs!


</p><h3>Input</h3>

<p align="justify">The input consists of <var>T</var> test cases. The number of them (<var>T</var>) is given on
the first line of the input file.
Each test case begins with a line containing two integers <var>E</var> and <var>F</var>. They
indicate the weight of an empty pig and of the pig filled with coins. Both
weights are given in grams. No pig will weigh more than 10 kg, that means
<var>1 &lt;= E &lt;= F &lt;= 10000</var>. On the second line of each test
case, there is an integer number <var>N</var>
(<var>1 &lt;= N &lt;= 500</var>) that gives the number of various
coins used in the given currency. Following this are exactly <var>N</var> lines,
each specifying one coin type. These lines contain two integers each, <var>P</var>and <var>W</var>
(<var>1 &lt;= P &lt;= 50000</var>, <var>1 &lt;= W &lt;=10000</var>).
<var>P</var> is the value of the
coin in monetary units, <var>W</var> is it's weight in grams.


</p><h3>Output</h3>

<p align="justify">Print exactly one line of output for each test case. The line must contain
the&nbsp;sentence 
"<code>The minimum amount of money in the piggy-bank is <var>X</var>.</code>"
where <var>X</var> is
the minimum amount of money that can be achieved using coins with
the given total weight. If the weight cannot be reached exactly,
print a&nbsp;line "<code>This is impossible.</code>".


</p><h3>Example</h3>
<pre>Sample Input:

3
10 110
2
1 1
30 50
10 110
2
1 1
50 30
1 6
2
10 3
20 4

Sample output:

The minimum amount of money in the piggy-bank is 60.
The minimum amount of money in the piggy-bank is 100.
This is impossible.
</pre>