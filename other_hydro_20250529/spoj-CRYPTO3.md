<p align="justify">
The Bytelandian cryptographer acknowledged he was sorely beaten in Act 2. He renounced his own methods of encryption and decided to return to the classic techniques.</p>
<p align="justify">
Not knowing what to do next, he went to the cinema to chew the problem over. To his surprise, he found that the cone containing pop-corn was in fact a rolled up page torn from the classic book, <i>RSA for newbies in 24 seconds</i>. The page in question contained the entire key-generating and encryption algorithm. Fascinated, he thought up two different prime numbers p and q, and calculated his own public key, and revealed the product p*q to the wide world. Then, he began work on his wicked scheme of encryption.
</p>
<p>
History repeats. Once more, you receive an encrypted message from the cryptographer. This time you know that without additional information you are beaten, so you decide to use the psychological approach. You phone the Bytelandian cryptographer, and ask him whether he couldn't give you a little hint. What you really want to know is the number u of positive integers which are smaller than p*q and have no common factors with p*q other than 1. But the cryptographer, sensing that this would allow you to decode the message right away, refuses to tell you this number. Eventually, after a lot of asking, he gives you a piece of utterly useless information: he tells you how many positive integers x cannot be represented in the form x=a*p+b*q, regardless of what non-negative integer values a and b assume.
</p><p>
You begin to wonder whether the information you received from the cryptographer is not by any chance enough to find the value of u.<br>
<b>Even if the only languages at your disposal are Brainf**k and Intercal...</b>
</p>
<h3>Input</h3>
<p align="justify">
The number provided by the cryptographer (a positive integer of at most 99 decimal digits). The input ends with a new line symbol.
</p>
<h3>Output</h3>
<p align="justify">
The value of u.
</p>
<h3>Example</h3>
<div align="left">
<pre><b><tt>Input:</tt></b>
1

<b><tt>Output:</tt></b>
2
</pre>
(This example is possible for p=2, q=3)</div>