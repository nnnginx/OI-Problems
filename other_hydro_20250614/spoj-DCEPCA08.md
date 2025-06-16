<p>Alice and Bob devised a new game to play. Alice wrote an expression on the paper and started generating an array of numbers from that. She wrote the formula as <br> a[i]=(51*a[i-1]+52)%53+1 <br> The array starts from index 1 and a[0]=1</p>
<p>Bob takes all the numbers from that array upto an index N also given by Alice. He makes all the subsets possible from that array. He calculates the sum of numbers in each of the subsets and finds which of the subset is prime.A subset is prime if the sum of numbers in the subset is a prime number.Bob gets boggled by the enormous size of array that alice is generating and asking him to do this.Can you help Bob calculate the number of different prime subsets that can be made from the given array ?</p>
<h3>Constraints</h3>
<p>0&lt;T&lt;=100<br> 0&lt;N &lt;=10^5</p>
<h3>Input</h3>
<p>It consists of T+1 lines were T is the number of test cases and N is the index of the array upto which Bob has to calculate. The array of the numbers can always be formed from the formula that Alice wrote.<br> Note : Array index starts from 1. Hence a[0] is not an element of the array.</p>
<h3>Output</h3>
<p>Print T lines each containing the number of different prime subsets that can be made from the array given.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>4<br>5<br><br>&nbsp;<strong>Output:</strong><br>3<br>6<br>&nbsp;</pre>