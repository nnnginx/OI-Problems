<pre style="font-family: 'Andale Mono', 'Courier New', Courier, monospace;"><code style="font-family: 'Andale Mono', 'Courier New', Courier, monospace;">**********************************************************************
                           GOLD PROBLEMS
**********************************************************************
                  Three problems numbered 1 through 3
**********************************************************************

Problem 1: Land Acquisition [Paul Christiano, 2007]

Farmer John is considering buying more land for the farm and has
his eye on N (1 &lt;= N &lt;= 50,000) additional rectangular plots, each
with integer dimensions (1 &lt;= width_i &lt;= 1,000,000; 1 &lt;= length_i
&lt;= 1,000,000).

If FJ wants to buy a single piece of land, the cost is $1/square
unit, but savings are available for large purchases. He can buy
any number of plots of land for a price in dollars that is the width
of the widest plot times the length of the longest plot. Of course,
land plots cannot be rotated, i.e., if Farmer John buys a 3x5 plot
and a 5x3 plot in a group, he will pay 5x5=25.

FJ wants to grow his farm as much as possible and desires all the
plots of land. Being both clever and frugal, it dawns on him that
he can purchase the land in successive groups, cleverly minimizing
the total cost by grouping various plots that have advantageous
width or length values.

Given the number of plots for sale and the dimensions of each,
determine the minimum amount for which Farmer John can purchase all

PROBLEM NAME: acquire

INPUT FORMAT:

* Line 1: A single integer: N

* Lines 2..N+1: Line i+1 describes plot i with two space-separated
        integers: width_i and length_i

SAMPLE INPUT:

4
100 1
15 15
20 5
1 100

INPUT DETAILS:

There are four plots for sale with dimensions as shown.

OUTPUT FORMAT:

* Line 1: The minimum amount necessary to buy all the plots.

SAMPLE OUTPUT:

500

OUTPUT DETAILS:

The first group contains a 100x1 plot and costs 100. The next group
contains a 1x100 plot and costs 100. The last group contains both the 20x5
plot and the 15x15 plot and costs 300. The total cost is 500, which is
minimal.</code></pre>