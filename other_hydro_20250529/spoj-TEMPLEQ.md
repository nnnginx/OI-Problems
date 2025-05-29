<table border="0">
<tbody>
<tr>
<td><img src="./24640/file/AAmf4qkJ.png" alt="main-destinations-tirupati" width="215" height="120"></td>
<td>
<p align="justify">The <a href="http://en.wikipedia.org/wiki/Tirumala_Venkateswara_Temple" target="_blank">Tirumala temple </a> is the most visited place of worship in the world. As the number of pilgrims who visit the temple each day is very high, the head of the temple should keep monitoring the queue system. Today is another lovely day and he has started his work. There are <strong>N</strong> queues at the entrance of the temple and some of them are already filled with pilgrims. Each queue has a metal door at the beginning, which leads to the temple. When the door is opened, it allows only one pilgrim to get through it and it gets closed immediately after that.</p>
</td>
</tr>
</tbody>
</table>
<p align="justify">New pilgrims are rushing in to the queues and the head needs to monitor the current sizes of the queues and decide which doors to be opened. At any time, he wants to know how many queues currently have at least <strong>X</strong> pilgrims. He also decides an integer <strong>Y</strong> and wants to open the doors of all the queues having at least <strong>Y</strong> pilgrims at that time. You are the controller of the queue system and are following his instructions. Respond quickly and win yourself a big laddu (sweet) from him :) .</p>
<p><br> Read the input section for rest of the details. <br><br></p>
<h3>Input</h3>
<p>The first line contains two integers N and Q. N - The number of queues [ 1 &lt;= N &lt;= 100,000 ], Q - The number of queries [ 0 &lt;= Q &lt;= 500,000 ] . The second line contains N integers, which are the initial sizes of the queues. ith integer ( 1-based ) is the initial size of queue i  [ 0 &lt;= initial size &lt;= 100,000,000 ] <br><br> Each of the next Q lines is one of the following <br><br> 1 A  [ One pilgrim enters the queue# A ( 1 &lt;= A &lt;= N ) ] <br><br> 2 X  [ Find the number of queues having atleast X pilgrims currently ( 0 &lt;= X &lt;= 1,000,000,000 )  ] <br> <br> 3 Y  [ Open the doors of all the queues having atleast Y pilgrims ( 1 &lt;= Y &lt;= 1,000,000,000 ), and thus allowing only one pilgrim to enter the temple from each of them ] <br><br></p>
<h3>Output</h3>
<p>For each query of type "2 X" , print the answer in a new line. <br><br></p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>5 6<br>20 30 10 50 40<br>2 31<br>1 2<br>2 31<br>3 11<br>2 20<br>2 50<br><br><strong>Output:</strong><br>2<br>3<br>3<br>0<br><br><strong>Note : Ideal time limit should be 2s. It has been increased to 7s, to let Java solutions pass, as the i/o is huge.</strong><br><br>* There are multiple test sets, and the judge shows the <strong>sum</strong> of the time taken over all test sets of your submission, if Accepted.</pre>