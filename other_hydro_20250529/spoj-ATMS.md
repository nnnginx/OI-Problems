<p align="justify">Every member of Byteland Credit Society is entitled to loan any amount of Bytelandish ducats unless it is 10<sup>30</sup> or more, but he has to return the whole amount within seven days. There are 100 ATMs in the Client Service Room of the Society. They are numbered from 0 to 99. Every ATM can perform one action only: it can pay or receive a fixed amount. The <i>i</i>-th ATM pays 2<i><sup>i</sup></i> ducats if <i>i</i> is even or it receives 2<i><sup>i</sup></i> ducats if <i>i</i> is odd. If a client is going to loan a fixed sum of money it is necessary to check if he is able to get the money using every ATM at most once. If so, numbers of ATMs he has to use should be determined. It is also necessary to check if the client can return the money in a similar way, and if so, to determine numbers of ATMs he has to use. </p>
<h3>Example</h3>
 <p align="justify">A client who is going to loan 7 ducats gets 16 ducats from the ATM # 4 and 1 ducat from the ATM # 0 and then he returns 8 ducats in the ATM # 3 and 2 ducats in the ATM # 1. In order to return the amount of 7 ducats he receives 1 ducat from the ATM # 0 and then he returns 8 ducats in ATM # 3. </p>

<h3>Task</h3>
<p align="justify">Write a program that:</p>
<div align="justify">
<ul align="justify">
        <li align="justify">reads the number of clients <i>n</i>, for every client reads from the same file the amount of money he is going to loan; </li>
        <li align="justify">checks for every client if he is able to get the money using every ATM at most once and if so, determines the numbers of ATMs he has to use; </li>
        <li align="justify">outputs the results. </li>
</ul></div>

<h3>Input</h3>
<p align="justify">In the first line of input there is one positive integer <i>n</i> &lt;= 10000, which equals the number of clients. </p>
 <p align="justify">In each of the following <i>n</i> lines there is one positive integer less than 10<sup>30</sup> (at most 30 decimal digits). The number in the <i>i</i>-th line describes the amount of ducats which the client <i>i</i> is going to loan. </p>

<h3>Output</h3>
<p align="justify">For each client you should output two lines with a decreasing sequence of positive integers from the range [0..99] separated by single spaces, or one word "<tt>No</tt>": </p>
<p align="justify">In the first line of the <i>i</i>-th pair of lines there should be numbers of ATMs (in decreasing order) that the client <i>i</i> should use to get his loan or one word "<tt>No</tt>" if the loan cannot be received according to the rules; </p>
<p align="justify">In the second line of the <i>i</i>-th pair there should be numbers of ATMs (in decreasing order) which the client <i>i</i> should use to return his loan or the word "<tt>No</tt>". </p>

<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
2
7
633825300114114700748351602698

<b><tt>Sample output:</tt></b>
4 3 1 0
3 0
No
99 3 1
</pre>