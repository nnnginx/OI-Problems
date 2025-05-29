<p>Gopu is playing with fishes, He likes playing them very much because they are lovely creatures. There are <b>n</b> fishes, All the <b>n</b> fishes are kept in n aquariums. Each fish is kept in different aquarium.</p>
<p>While he is playing with them, there comes a magic instant in his play. At that instant, fish in aquarium <b>i</b> can go to aquarium <b>j</b> with probability p[i][j]. At this magic instant, all the fishes go to aquariums according to their probabilities.</p>
<p>Now there is a slight issue in this, If more than one fishes land on the same aquarium, Then they can not survive because of lack of space. You have to find the probability that none of Gopu's fishes dies, otherwise he would be very sad.&nbsp;</p>
<p>Please help our little Gopu so that he could keep playing with his fishes :)</p>
<h3>Input</h3>
<p>First line contains number of test cases : T (1 &lt;= T &lt;= 1000)</p>
<p>Next line contains n : number of fishes (1 &lt;= n &lt;= 15).</p>
<p>For next n lines, each line contains n space seperated real numbers. In line i, jth number is p[i][j]. p[i][j] is precise upto 6 decimal digits.</p>
<h3>Output</h3>
<p>For each test case, print the probability that none of Gopu's fishes dies. (probability is a real number and it should not have error more than 1e-6), That is your answer should be correct upto 6 decimal digits.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>2<br>1 0<br>0 1<br>2<br>0.5 0.5<br>0.5 0.5

<strong>Output:</strong>
1.000000<br>0.500000
</pre>