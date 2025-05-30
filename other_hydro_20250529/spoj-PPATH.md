<p>
<img src="./23944/file/hK56klIp.png">
</p>
<p>
The ministers of the cabinet were quite upset by the 
message from the Chief of Security stating that they
would all have to change the four-digit room numbers 
on their offices. <br>
！ It is a matter of security to change such things
    every now and then, to keep the enemy in the dark.<br>
！ But look, I have chosen my number 1033 for good
    reasons. I am the Prime minister, you know!<br>
！ I know, so therefore your new number 8179 is also
    a prime. You will just have to paste four new
    digits over the four old ones on your office door.<br>
！ No, it's not that simple. Suppose that I change the
    first digit to an 8, then the number will read 8033
    which is not a prime!<br>

！ I see, being the prime minister you cannot stand
    having a non-prime number on your door even for a
    few seconds.<br>
！ Correct! So I must invent a scheme for going from
    1033 to 8179 by a path of prime numbers where
    only one digit is changed from one prime to the
    next prime.

</p><p>
Now, the minister of finance, who had been eavesdropping,
intervened.<br>
！ No unnecessary expenditure, please! I happen to
    know that the price of a digit is one pound.<br>
！ Hmm, in that case I need a computer program to 
    minimize the cost. You don't know some very cheap
    software gurus, do you?<br>
！ In fact, I do. You see, there is this programming
    contest going on...
</p>
<p>

Help the prime minister to find the cheapest prime path
between any two given four-digit primes! The first digit
must be nonzero, of course. Here is a solution in the 
case above.
</p><pre>    1033
    1733     
    3733     
    3739     
    3779
    8779
    8179     
</pre>
The cost of this solution is 6 pounds.  Note that the digit 1
which got pasted over in step 2 can not be reused in the last step
�C a new 1 must be purchased.
<p></p>
<h3>Input</h3>
<p>
One line with a positive number: the number of test cases (at most
100). Then for each test case, one line with two numbers separated by
a blank.  Both numbers are four-digit primes (without leading zeros).
</p>
<h3>Output</h3>
<p>One line for each case, either with a number stating the minimal cost
or containing the word <tt>Impossible</tt>. 
</p>
<h3>Example</h3>

<pre><b>Input:</b>
3
1033 8179
1373 8017
1033 1033

<b>Output:</b>
6
7
0
</pre>