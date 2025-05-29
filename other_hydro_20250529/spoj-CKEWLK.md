<p style="text-align: justify;">In a country called STI Countries (STI stands for Super Toxicity Inc.), there is one day dedicated for the people to do everything they want. This day is called FREE DAY. Of course they must keep their activites not to violate the law. For example, everything that lead to criminality is forbidden because it violates the law.</p>
<p style="text-align: justify;">The president of STI Countries is very excited to <strong>FREE DAY</strong>. For him, being a president made him as the busiest man in the world, so holiday is almost impossible for him, even Sunday. But, FREE DAY gives him a chance to feel freedom from all of his duty as the president.</p>
<p style="text-align: justify;">For this FREE DAY, president and his family want to make a party. This party is called Cake Walk Party. As it namesake, this party will have relation with cakes. So, president needs a talented baker for the best cakes he want. Then, the president called Brembo, the best baker in the country. Called by the president, the baker will make sure the cakes he made would impress the president. The president will order <strong>T</strong> cakes<strong>, </strong>with every of them is different type. To make a cake, Brembo needs <strong>M </strong>package of ingredients. The type of a cake will be represented by a number that is <strong>N</strong>. After doing some experiments, he finds a good formula to make the ingredients of cake with type <strong>N</strong>. He called this F(N).</p>
<p style="text-align: justify;">He writes the fomula F(N) as F(N) = F(1) + F(2) + F(3) + F(4) + ..... + F(N-1) with F(1) = M.</p>
<p>Normally, the cake with type N, will be priced C(N) in dollars, where C(N) = M + N + F(N). But, because today is a special day plus he is doing job for the president, the way of pricing a cake is different than before. He makes rules as the following :</p>
<ol style="text-align: justify;"> </ol> 
<ul>
<li>From C(N), find all special factor of C(N).</li>
<li>Because Brembo is not good at explaining, Brembo defines special factor of a number with examples. For example 24, the special factors are 2<sup>3</sup> and 3. For 15, special factors are 3 and 5. And so on.</li>
</ul>
<ol style="text-align: justify;"> </ol> 
<ul>
<li>Then, the price of the cake will be taken from factor with the highest value. So, from the example above, 24 will be priced 3 instead.</li>
<li>So far, 15 will be priced 5 instead.</li>
</ul>
<ol style="text-align: justify;"> </ol>
<p>Considering the results of C(N) can be very large, he does C(N) mod 1000000007 for every C(N) he calculates, then factorize it. As the assisstant of Brembo, you need to calculate the total cost that president must pay for the <strong>T</strong> cakes he orders. Because this task will be exhausting, you build a program to make the calculation faster.</p>
<h3 style="text-align: justify;">Input</h3>
<p style="text-align: justify;">The first line of input consist of two integers, <strong>T</strong> and <strong>M</strong> separated by space. T represents the number of cake that The President will order and M represents the package of ingredients. (1 &lt;= T &lt;= 100 and 1 &lt;= M &lt;= 1000000)</p>
<p style="text-align: justify;">The next T lines, contains one integer <strong>N</strong>i, representing the type number of cakes. ( 1 &lt;= N &lt;= 1000000)</p>
<h3 style="text-align: justify;">Output</h3>
<p style="text-align: justify;">Print the total cost that The President must pay using the following format : "The President needs to pay (total) dollar(s)" without quotes.</p>
<p style="text-align: justify;">Please, take a look to example.</p>
<h3 style="text-align: justify;">Example</h3>
<pre style="text-align: justify;"><strong>Input:</strong>
3 11
2
3
4

<strong>Output:</strong>
The President needs to pay 65 dollar(s)
</pre>