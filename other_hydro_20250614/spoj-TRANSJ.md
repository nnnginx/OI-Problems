<p>Ruratania is just entering capitalism and is establishing new enterprising activities in many fields including transport. The transportation company TransRuratania is starting a new express train from city A to city B with several stops in the stations on the way. The stations are successively numbered, city A station has number 0, city B station number&nbsp;<em>m</em>. The company runs an experiment in order to improve passenger transportation capacity and thus to increase its earnings. The train has a maximum capacity&nbsp;<em>n</em>&nbsp;passengers. The price of the train ticket is equal to the number of stops (stations) between the starting station and the destination station (including the destination station). Before the train starts its route from the city A, ticket orders are collected from all onroute stations. The ticket order from the station S means all reservations of tickets from S to a fixed destination station. In case the company cannot accept all orders because of the passenger capacity limitations, its rejection policy is that it either completely accept or completely reject single orders from single stations.</p>
<p>&nbsp;</p>
<p>Write a program which for the given list of orders from single stations on the way from A to B determines the biggest possible total earning of the TransRuratania company. The earning from one accepted order is the product of the number of passengers included in the order and the price of their train tickets. The total earning is the sum of the earnings from all accepted orders.</p>
<p>&nbsp;</p>
<h2><span style="color: #000000;"><a name="SECTION0001001000000000000000">Input</a></span></h2>
<p>The input file is divided into blocks. The first line in each block contains three integers: passenger capacity&nbsp;<em>n</em>&nbsp;of the train, the number of the city B station and the number of ticket orders from all stations. The next lines contain the ticket orders. Each ticket order consists of three integers: starting station, destination station, number of passengers. In one block there can be maximum 22 orders. The number of the city B station will be at most 7. The block where all three numbers in the first line are equal to zero denotes the end of the input file.</p>
<p>&nbsp;</p>
<h2><span style="color: #000000;"><a name="SECTION0001002000000000000000">Output</a></span></h2>
<p>The output file consists of lines corresponding to the blocks of the input file except the terminating block. Each such line contains the biggest possible total earning.</p>
<p>&nbsp;</p>
<h2><span style="color: #000000;"><a name="SECTION0001003000000000000000">Sample Input</a></span></h2>
<pre>10 3 4
0 2 1
1 3 5
1 2 7
2 3 10
10 5 4
3 5 10
2 4 9
0 2 5
2 5 8
0 0 0</pre>
<p>&nbsp;</p>
<h2><span style="color: #000000;"><a name="SECTION0001004000000000000000">Sample Output</a></span></h2>
<pre>19
34</pre>