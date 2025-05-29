<h3>Background</h3>
<p>This problem is somewhat easier than the problem <a href="http://www.spoj.com/problems/EASYPROB">A Very Easy Problem!</a> because of the super long time limit...</p>
<h3>Description</h3>
<p>Assurance Company of Moving (ACM) is a company of moving things for people. Recently, some schools want to move their computers to another place. So they ask ACM to help them. One school reserves <em>K</em> trucks for moving, and it has <em>N</em> computers to move. In order not to waste the trucks, the school ask ACM to use all the trucks. That is to say, there must be some computers in each truck, and there are no empty trucks. ACM wants to know how many partition shemes exists with moving N computers by K trucks, the ACM ask you to compute the number of different shemes with given N and K. You needn't care with the order. For example <em>N</em>=7,<em>K</em>=3, the the following 3 partition instances are regarded as the same one and should be counted as one sheme: "1 1 5","1 5 1","5 1 1". Each truck can carry almost unlimited computers!!</p>
<h3>Input</h3>
<p>Each line of the input contains two postisive integer N (1&lt;=N&lt;=5000) and K(1&lt;=K&lt;=N).Input is terminated by a line with N=K=0(this case should not be processed).</p>
<h3>Output</h3>
<p>For each line, output the number of different partition sheme. To avoid big integers, you may output the answer modudo 1988.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>1 1<br>7 3<br>0 0<br><br><strong>Output:</strong><br>1<br>4<br></pre>