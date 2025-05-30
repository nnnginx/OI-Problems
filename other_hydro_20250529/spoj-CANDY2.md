<p>Little Michael loves candies. Most of all, he likes chocolate, strawberry and banana flavored ones. No wonder that he has candy bags everywhere - there are at least four bags on his table, one or two in the pockets of his jeans, and one under his bed (just in case). Each bag contains some candies of all three flavors. Whenever he wants to eat a candy, he finds the nearest bag (which is usually is not very far because he has really A LOT of them) and eats the candy he wants.</p> 

<p>Yesterday, he wanted a strawberry one, so he opened one of his bags and... It is almost impossible to describe how great his disappointment was when he found out that there were no strawberry candies left in that bag. To make the matters worse, there were also none in the second bag he found. He was sure that he had lots of strawberry candies left, but he didn't know in which bags they were. Therefore, he decided to reorganize his candies, and keep the candies of the three different flavors in three distinct bags. He brought all his bags into the center of his room and realized, that there are really an awful lot of them. </p>

<p>Michael has N bags full of candies. He knows the number of candies of each flavor in each bag. He wants to put all chocolate ones into one bag, all strawberry ones into another bag and all banana ones into yet another bag. He has to move the candies one-by-one, because he always has to look at it to determine its flavor. Moving one candy from one bag into another takes 1 second. Your task is to select the bag for each flavor, so that the total time required for Michael to move all the candies into their bags would be minimal. </p>

<h3>Input file specification</h3>
<p>The first line of the input file contains a single integer N - the number of bags (N&lt;=5000). Each of the following N lines consists of three numbers ci, si, bi - the numbers of chocolate, strawberry and banana candies in the i-th bag. The bags are numbered from 0 to N-1 in the order in which they appear in the input. </p>

<h3>Output file specification</h3>
<p>Output file should contain three lines with the following text: </p>
<pre>C[Bag for chocolate candies]
S[Bag for strawberry candies]
B[Bag for banana candies]
</pre>
<p>The numbers C, S, B have to be such that the total number of the required moves is minimal. If there are more solutions, you may choose any of them.</p>

<h3>Example</h3>
<pre><b>Input file:</b>
5
10 10 10
40 39 40
10 20 30
30 20 10
1 2 27

<b>Output file:</b>
3
1
2
</pre>
<p>Note: In this case Michael has to move 200 candies. If the bags for the different flavors were chosen in any other way, he would have to move more than 200 candies. </p>
<b>Note: the test data is very naive for this problem.</b>