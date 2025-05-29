<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/MSE07B/en/">English</a></td> 
<td width="50%"><a href="/problems/MSE07B/vn/">Vietnamese</a></td> 
</tr></tbody></table>

<p></p><p>
The new founded Balkan Investment Group Bank (BIG-Bank) opened a new 
office in Bucharest, equipped with a modern computing environment 
provided by IBM Romania, and using modern information technologies. </p><p>
As usual, each client of the bank is identified by a positive 
integer K and, upon arriving to the bank for some services, 
he or she receives a positive integer priority  P. One of the inventions 
of the young managers of the bank shocked the software 
engineer of 
the serving system. They proposed to break the tradition by sometimes 
calling the serving desk with the lowest priority instead of that with
 the highest priority. Thus, the system will receive the following types 
of request: </p><p>
0  The system needs to stop serving </p><p>
1  K P Add client K to the waiting list with priority P </p><p>
2  Serve the client with the highest priority and drop him or her 
from the waiting list </p><p>
3  Serve the client with the lowest priority and drop him or her from 
the waiting list.</p><p>
Your task is to help the software engineer of the bank by writing a 
program to implement the requested serving policy.  
</p><p>
</p><h3>Input</h3>
<p></p><p>
Each line of the input contains one of the possible requests; only 
the last line contains the stop-request (code 0). You may assume that 
when there is a request to include a new client in 
the list 
(code 1), there is no other request in the list of the same client 
or with the same priority. </p><p>
An identifier K is always less than 10^6, and a priority P is less 
than 10^7.The client may arrive for being served multiple times, and each 
time may obtain a different priority.
</p><p>
</p><h3>Output</h3>
<p></p><p>
For each request with code 2 or 3, the program has to print, in a 
separate line of the standard output, the identifier of the served 
client. If the request arrives when the waiting list is empty, then the 
program prints zero (0) to the output. 
</p><p>
</p><h3>Sample</h3>
<pre>Input :
2 
1 20 14 
1 30 3 
2 
1 10 99 
3 
2 
2 
0 
Ouput: 
0 
20 
30 
10 
0 
</pre>