<p><span style="white-space: normal;"> </span></p>
<p style="font-size: 13px; text-align: justify; color: #000020; background-color: #f6f9e0;">The concept of cloud computing has become fairly popular lately. One of the main kinds of cloud computing is known as IaaS (<em>Infrastructure as a Service</em>), in which servers can be rented and managed via the Internet.</p>
<p style="font-size: 13px; text-align: justify; color: #000020; background-color: #f6f9e0;">Cloud, Inc. is an IaaS provider. The company is designing a new data center for its clients. Through some research, they found out that their clients, as a whole, need K servers, each of which needs to be able to withstand a certain level of demand.&nbsp;If we assume that the cost of a server always grows with the demand which that server can process, the best solution in terms of cost is to buy K servers explicitly designed to meet the exact requirements of the corresponding client.</p>
<p style="font-size: 13px; text-align: justify; color: #000020; background-color: #f6f9e0;">However, having K different hardware configurations in the data center is extremely problematic for the system administrators. To simplify, they demand that no more than L distinct server types be bought. A server that meets a demand c also meets any demand smaller than c.</p>
<p style="font-size: 13px; text-align: justify; color: #000020; background-color: #f6f9e0;">A possible solution is to buy only one server type that is able to meet the highest client demand, as it will also be able to meet all other demands. On the other hand, the cost of such a solution can be prohibitively high. Considering that you can buy up to L different kinds of servers, there's likely a better option. For instance, suppose that there are 3 clients, with demands 3, 7 and 16. Assume that the cost of a server meeting demands up to 3 is of R$ 1500 (1500 brazilian reais), the cost of a server that meets demand 7 is R$ 5500 and the cost of a server that meets demand 16 is R$ 19200. If you want to buy at most 2 kinds of servers to satisfy all clients, you have four possibilities:</p>
<ul style="font-size: 13px; text-align: justify; color: #000020; background-color: #f6f9e0;">
<li>Buying three servers with capacity 16, at a total cost of R$ 57600;</li>
<li>Buying two servers with capacity 16 and one with capacity 7, at a total cost of R$ 43900;</li>
<li>Buying two servers with capacity 16 and one with capacity 3, at a total cost of R$ 39900;</li>
<li>Buying one server with capacity 16 and two servers with capacity 7, at a total cost of R$ 30200.</li>
</ul>
<p style="font-size: 13px; text-align: justify; color: #000020; background-color: #f6f9e0;">Among these options, the one with the least total cost is the last one.</p>
<p style="font-size: 13px; text-align: justify; color: #000020; background-color: #f6f9e0;">You will receive a list of K requested demands and the price of a server type that meets the corresponding demand. Determine the lowest total cost to buy K servers in a way such that all requested demands are met and at most L different types of servers are bought.</p>
<h3 style="font-size: 15px; color: #000020; text-align: center; background-color: #f6f9e0;">Notes</h3>
<p>&nbsp;</p>
<li style="text-align: left;">Each server is used by one and only one client. A server with capacity 4 may <strong>not</strong> be used by two clients with demand 2 each.</li>
<li style="text-align: left;">Let D<sub>i</sub>&nbsp;and D<sub>j</sub>&nbsp;be two demands, and P<sub>i</sub>, P<sub>j</sub>&nbsp;prices associated to the servers that meet those demands. If D<sub>i</sub>&nbsp;&lt; D<sub>j</sub>, then P<sub>i</sub>&nbsp;�� P<sub>j</sub>.</li>
<p>&nbsp;</p>
<h3 style="font-size: 15px; color: #000020; text-align: center; background-color: #f6f9e0;">Input</h3>
<p style="font-size: 13px; text-align: justify; color: #000020; background-color: #f6f9e0;">There are several test cases.</p>
<p style="font-size: 13px; text-align: justify; color: #000020; background-color: #f6f9e0;">Each test case begins with a line containing integers K and L, respectively the number of servers to be bought and the maximum allowed number of distinct server types (1 �� L �� K �� 2000). K lines follow, each of which containing two integers D and P, respectively the demand of a client and the smallest price of a server which meets that demand (1 �� D �� 2000, 1 �� P �� 100000). If the same value of D is present on more than one line, then both lines will have the same value for P.</p>
<p style="font-size: 13px; text-align: justify; color: #000020; background-color: #f6f9e0;">The input ends when K = L = 0, and this case should not be processed.</p>
<h3 style="font-size: 15px; color: #000020; text-align: center; background-color: #f6f9e0;">Output</h3>
<p style="font-size: 13px; text-align: justify; color: #000020; background-color: #f6f9e0;">For each test case, print a line with an integer T, which is the lowest total cost obtainable.</p>
<h3 style="font-size: 15px; color: #000020; text-align: center; background-color: #f6f9e0;">Example</h3>
<pre style="font-size: 13px; color: #000020; background-color: #f6f9e0;"><strong>Input:</strong>
10 3
1 1
2 4
3 5
4 7
5 8
6 12
7 13
8 18
9 19
10 21
0 0

<strong>Output:</strong>
129
</pre>
<p style="font-size: 13px; text-align: justify; color: #000020; background-color: #f6f9e0;">The best option to buy servers of 3 kinds that meet the required demands is to buy:</p>
<ul style="font-size: 13px; text-align: justify; color: #000020; background-color: #f6f9e0;">
<li>3 servers of capacity 10, which account for client demands 10, 9 and 8;</li>
<li>2 servers of capacity 7, which account for client demands 7 and 6;</li>
<li>5 servers of capacity 5, which account for all other demands.</li>
</ul>
<p style="font-size: 13px; text-align: justify; color: #000020; background-color: #f6f9e0;">Total cost is 3*21 + 2*13 + 5*8 = 129.</p>
<p>&nbsp;</p>