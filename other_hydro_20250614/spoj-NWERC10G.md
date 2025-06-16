<p>As you may know, the country of Absurdistan is full of abnormalities. For example, the whole country can be divided into unit squares that are either grass or swamp. Also, the country is famous for its incapable bureaucrats. If you want to buy a piece of land (called a parcel), you can only buy a rectangular area, because they cannot handle other shapes. The price of the parcel is determined by them and is proportional to the perimeter of the parcel, since the bureaucrats are unable to multiply integers and thus cannot calculate the area of the parcel.</p>
<p>Per owns a parcel in Absurdistan surrounded by swamp and he wants to sell it, possibly in parts, to some buyers. When he sells a rectangular part of his land, he is obliged to announce this to the local bureaucrats. They will first tell him the price he is supposed to sell it for. Then they will write down the name of the new owner and the coordinates of the south-east corner of the parcel being sold. If somebody else already owns a parcel with a south-east corner at the same spot, the bureaucrats will deny the change of ownership.</p>
<p>Per realizes that he can easily trick the system. He can sell overlapping areas, because bureaucrats only check whether the south-east corners are identical. However, nobody wants to buy a parcel containing swamp.</p>
<p style="text-align: center;"><img src="../../content/disatoba:NWERC10G" alt="" width="300" height="359"></p>
<p style="text-align: left;">Now Per would like to know how many parcels of each perimeter he needs to sell in order to maximize his profit. Can you help him? You may assume that he can always find a buyer for each piece of land, as long as it doesn't contain any swamps. Also, Per is sure that no square within his parcel is owned by somebody else.</p>
<h3>Input</h3>
<p>On the first line a positive integer: the number of test cases, at most 100. After that per test case:</p>
<ul>
<li>One line with two integers n and m (1 ¡Ü n, m ¡Ü 1&nbsp;000): the dimensions of Per's parcel.</li>
<li>n lines, each with m characters. Each character is either `<tt>#</tt>' or `<tt>.</tt>'. The j-th character on the i-th line is a `<tt>#</tt>' if position (i, j) is a swamp, and `<tt>.</tt>' if it is grass. The north-west corner of Per's parcel has coordinates (1, 1), and the south-east corner has coordinates (n,m).</li>
</ul>
<p>&nbsp;</p>
<h3>Output</h3>
<p>Per test case:</p>
<ul>
<li>Zero or more lines containing a complete list of how many parcels of each perimeter Per needs to sell in order to maximize his profit. More specifically, if Per should sell p</li>
</ul>
<h3>Example</h3>
<pre><strong>Input:</strong>
<pre>1
6&nbsp;5
..#.#
.#...
#..##
...#.
#....
#..#.</pre>
<strong>Output:</strong>
<pre>6&nbsp;x&nbsp;4
5&nbsp;x&nbsp;6
5&nbsp;x&nbsp;8
3&nbsp;x&nbsp;10
1&nbsp;x&nbsp;12</pre>
</pre>