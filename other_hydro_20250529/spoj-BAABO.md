<p>The 2*N (3 &lt;= N &lt;= 1,000) cows have assembled the Bovine Accordion and Banjo Orchestra!  They possess various levels of skill on their respective instruments: accordionist i has an associated talent level A<sub>i</sub> (0 &lt;= A<sub>i</sub> &lt;= 1,000); banjoist j has an associated talent level B<sub>j</sub> (0 &lt;= B<sub>j</sub> &lt;= 1,000).</p>
<p>The combined A<img style="vertical-align: middle;" title="awesomeness' of a pairing between cows with talents A" src="../../../files/gif/%5Cdisplaystyle%7Ba%7D%7Bw%7D%7Be%7D%7Bs%7D%7Bo%7D%7Bm%7D%7Be%7D%5Cne%7Bs%7D%7Bs%7D%27%7Bo%7D%7Bf%7B%7Ba%7D%7D%7D%7Bp%7D%7Ba%7D%7Bi%7D%7Br%7D%5Cin%7Bg%7B%7Bb%7D%7D%7D%7Be%7D%7Bt%7D%7Bw%7D%7Be%7D%7Be%7D%7Bn%7D%7Bc%7D%7Bo%7D%7Bw%7D%7Bs%7D%7Bw%7D%7Bi%7D%7Bt%7D%7Bh%7D%7Bt%7D%7Ba%7D%5Cle%7Bn%7D%7Bt%7D%7Bs%7D%7BA%7D" alt=""><sub>i</sub> and B<sub>j</sub> is directly proportional to the talents of each cow in the pair so a concert with those two cows will earn FJ precisely A<sub>i</sub> * B<sub>j</sub> dollars in "charitable donations".  FJ wishes to maximize the sum of all revenue obtained by his cows by pairing them up in the most profitable way.</p>
<p>Unfortunately, FJ's accordionists are a bit stuck up and stubborn. If accordionist i is paired with banjoist j, then accordionists i+1..N refuse to be paired with banjoists 1..j-1. This creates restrictions on which pairs FJ can form. FJ thus realizes that in order to maximize his profits, he may have to leave some cows unpaired.</p>
<p>To make matters worse, when one or more of the musicians is skipped, they will be greatly upset at their wasted talent and will engage in massive binge drinking to wash away their sorrows.</p>
<p>After all pairings are made, a list is constructed of the groups of each of the consecutive skipped musicians (of either instrument). Every group of one or more consecutive skipped cows will gather together to consume kegs of ice cold orange soda in an amount proportional to the square of the sum of their wasted talent.</p>
<p>Specifically, FJ has calculated that if the x-th to y-th accordionists are skipped, they will consume precisely (A<sub>x</sub> + A<sub>x+1</sub> + A<sub>x+2</sub> + ... + A<sub>y</sub>)<sup>2</sup> dollars worth of orange soda in the process of drinking themselves into oblivion. An identical relationship holds for the banjoists. FJ realizes that he'll end up getting stuck with the bill for his cows' drinking, and thus takes this into account when choosing which pairings to make.</p>
<p>Find the maximum amount of total profit that FJ can earn after the contributions are collected and the orange soda is paid for.</p>
<h3>Input</h3>
<p>* Line 1: A single integer: N</p>
<p>* Lines 2..N+1: Line i+1 contains the single integer: A<sub>i</sub></p>
<p>* Lines N+2..2*N+1: Line i+N+1 contains the single integer: B<sub>i</sub></p>
<h3>Output</h3>
<p>* Line 1: A single integer that represents the maximum amount of cash         that FJ can earn.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
1
1
5
5
1
1

<strong>Output:</strong>
17
</pre>
<p><strong>Explanation</strong></p>
<p>There are 6 cows: 3 accordionists and 3 banjoists. The accordionists have talent levels (1, 1, 5), and the banjoists have talent levels (5, 1, 1).</p>
<p>FJ pairs accordionist 3 with banjoist 1 to get earn A<sub>3</sub> * B<sub>1</sub> = 5 * 5 = 25 in profit.  He loses a total of (1 + 1)<sup>2</sup> + (1 + 1)<sup>2</sup> = 8 dollars due to the cost of soda for his remaining cows. Thus his final (net) profit is 25 - 8 = 17.</p>