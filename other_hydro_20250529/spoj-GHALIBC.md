<p>"har ek baat pe kehte ho tum ke 'too kya hai?'<br>tumheen kaho ke yeh andaaz-e-guftgoo kya hai?"

</p><p>Ghalib was a great poet and was very higly regarded by the emperor. Some of the nobles did not like this, so concocted a plan to reduce his influence on the emperor. They gave him a challenge, he could be given n bags of marbles. The first bag has 1 marble, second bag has 2 marbles and so on. Each of the marble has a unique radius between 1 and i, where i is the number of the bag. Ghalib has to tell the number of ways arranging these marbles. (The marbles in each of the bag have to be arranged separately and the number of ways summed up for all the bags).

</p><p>Ghalib complained to the king that this task is too difficult. So the king tried to help him a bit. (n+1) will only be divisible by a single prime - p (i.e. (n+1)=p^a) and he has to only find ways of rearranging those bags of marbles whose size is equal to r mod(p-1) and (p+1)/2&lt;=r&lt;=p-1. Also he doesnt need to count any arrangement of marbles containing a subsequence of 3 marbles with increasing length.<br>Ghalib still finds this task too difficult and is asking for your help. Since the answer can be very big, output the remainder when the answer is divided by p*p.</p>
<h3>Input</h3>
<p>1&lt;=t&lt;=10 :-&nbsp; the number of test cases</p>
<p>followed by t llines of</p>
<p>r p a :- as given in the question</p>
<p>(p+1)/2&lt;=r&lt;=p-1</p>
<p>5&lt;=p&lt;=1000</p>
<p>1&lt;=a&lt;=10^8</p>
<h3>Output</h3>
<p>A single number representing the required answer</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>5 7 2<br>5 7 1

<strong>Output:</strong><br>42<br>42</pre>