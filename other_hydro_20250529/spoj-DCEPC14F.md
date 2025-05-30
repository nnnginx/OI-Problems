<p>One day Amit had an idea to open up a toy store. Though he realised that he must do something to attract customers to his store otherwise his store would not be successful. So he comes up with a plan to give each customer a free Lego (blocks) set. Hearing about this, you go to the store to get your free sample. <br><br>You are provided with a set of Legos. The set given to you consists of N different kinds of legos. The set has an infinite number of pieces of each kind of Lego. Each kind of Lego has some fixed height. Note that 2 different kinds of Legos may have the same height.<br><br>Now you want to check the actual price of your Lego set. The price of the set is equal to the number of distinct Beautiful Buildings that can be built using the set.<br><br>A Beautiful Building is a stack of Lego pieces such that it is made of exactly K Lego pieces (not necessarily of different kind) and it's height is equal to X modulo M for given values of X, M and K(These values are printed on the Box).<br><br>2 Buildings are distinct if there exists a height H at which the block used in both buildings is not the same.<br><br>You want to find out the price of the free sample provided to you.</p>
<h3>Input</h3>
<p>The input starts with an integer T , indicating the number of test cases. Then T test cases follow. Each test cases consists of 3 lines. The first line contains an integer N , indicating the number of different kinds of legos in the set. The second line contains N space separated integers , the ith of which represents the height of peices of ith kind. The third line contains 3 space separated integers representing the values of M,K and X respectively.</p>
<h3>Output</h3>
<p>For each test case print a line containing the price of the set modulo 1000000007.</p>
<p>&nbsp;</p>
<p><strong>CONSTRAINTS</strong><br><br>T&lt;=100<br>1&lt;=N&lt;=100000<br>1&lt;=M&lt;=100<br>1&lt;=K&lt;=1000000000<br>0&lt;=X&lt;M<br>1&lt;=Height of Each Lego&lt;=1000000000</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>2<br>3<br>1 2 3<br>3 1 0<br>3<br>1 2 3<br>3 2 0

<strong>Output:</strong>
1<br>3 <br></pre>