<p>There are <i>n</i> dealers in the market. Each of them has some unique goods (nobody else has the same goods). Besides, each of them wants to obtain some other goods, which exist in the market. This is rather strange, but for each kind of goods on the market there exists exactly one dealer who wants to obtain it.<br><br>

To prevent fraud, only exchanges in pairs are allowed in this market. Moreover, each dealer is allowed to make at most one exchange a day. But the total number of transactions isn¡¯t limited. A transaction means that all the goods of one dealer are exchanged for all the goods of the other participating dealer (partial transactions are not allowed).<br><br>

You are to write a program which outputs the minimum number of days needed for each dealer to get the goods that he wants. Also output one of the possible variants of exchanges leading to this goal.<br>

</p><h3>Input</h3>
<p> The first line contains an integer <i>n</i> [<i>n</i> &lt;= 5000]. In the second line exactly <i>n</i> numbers of goods are given, which the dealers require. If integer <i>j</i> appears as the <i>i</i>-th at input, then this means that goods required by dealer <i>i</i> are initially owned by dealer <i>j</i>.</p>
 
<h3>Output</h3>
<p>You must output the minimum number of days <i>m</i> which are needed to complete the transactions. In the next <i>m</i> lines you must output the way these transactions should be managed by the dealers. One line corresponds to one day. At the beginning of each line you must output the number of transactions on this day. After that output the pairs of dealers who exchange their goods on this day. Dealers in pairs are separated by '-' symbol. If there are many ways to perform the exchanges then output any of them.</p>

<h3>Example</h3>

<pre><b>Input:</b>
7
2 1 3 5 6 7 4

<b>Output:</b>
2
3 1-2 4-5 7-6
1 5-7
</pre>

<h3>Author: Filimonenkov D.O.</h3>