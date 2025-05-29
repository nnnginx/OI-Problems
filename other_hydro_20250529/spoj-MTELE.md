<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/MTELE/en/">English</a></td> 
<td width="50%"><a href="/problems/MTELE/vn/">Vietnamese</a></td> 
</tr></tbody></table>

<p>
A TV-network plans to broadcast an important football match. Their
network of transmitters and users can be represented as a  tree. The
root of the tree is a transmitter that emits the football match, the 
leaves of the tree are the potential users and other vertices 
in the tree are relays (transmitters). 
The price of transmission of a signal from one transmitter 
to another or to the user is given. A price of 
the entire 
broadcast is the sum of prices of all individual signal transmissions. 
Every user is ready to pay a certain amount of money to watch the 
match and the TV-network then decides whether or not to provide the
user with the signal. 
Write a program that will find the maximal number of users able 
to watch the match so that the TV-network¡¯s doesn¡¯t lose money from 
broadcasting the match.
  
</p>
<h3>Input</h3>
<p>
The first line of the input file contains two integers N and M, 2 ¡Ü N ¡Ü 3000,
1 ¡Ü M ¡Ü N-1, the number of vertices in the tree and the number of 
potential users. 
The root of the tree is marked with the number 1, while other transmitters
are numbered 2 to N-M and potential users are numbered N-M+1 to N. 
The following N-M lines contain data about the transmitters 
in the following form: 
K A1 C1 A2 C2 ... AK CK 
Means that a transmitter transmits the signal to K transmitters or 
users, every one of them described by the pair of numbers A and C, the 
transmitter or user¡¯s number and the cost of transmitting the signal to 
them. 
The last line contains the data about users, containing M integers 
representing respectively the price every one of them is willing to 
pay to watch the match.
</p>
<h3>Output</h3>
<p>
The first and the only line of the output file should contain the 
maximal number of users described in the above text. 
</p>
<h3>Sample</h3>
<pre>tele.in 
 
5 3 
2 2 2 5 3 
2 3 2 4 3 
3 4 2 
 
tele.out 
 
2 

tele.in 
 
5 3 
2 2 2 5 3 
2 3 2 4 3 
4 4 2 
 
tele.out 
 
3 

tele.in 
 
9 6 
3 2 2 3 2 9 3 
2 4 2 5 2 
3 6 2 7 2 8 2 
4 3 3 3 1 1 
 
tele.out 
 
5
</pre>