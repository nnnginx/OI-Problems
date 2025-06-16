A standard deck of cards has <strong>52</strong> cards in total, <strong>4</strong> suits - Hearts, Diamonds, Clubs, and Spades and each suit has <strong>13</strong> cards (<strong>2, 3, 4, 5, 6, 7, 8, 9, 10, Jacks, Queens, Kings and Aces</strong>). Oompa Loompa is an amateur magician who loves card magics. As you know, many magic tricks are rather simple once you know the secret behind them. Oompa Loompa's favorite trick is the random magic trick. The trick goes on like this. At first, he takes a deck of cards consisting of some suits, and each suit containing some cards, and randomly shuffles them. The magician's trick here is to show there are at least <strong>2</strong> consecutive Kings as well as <strong>2</strong> consecutive Queens in the shuffled deck. As you can see, this trick relies on pure luck, and may be unsuccessful if the magician's luck runs out :)
<br><br>

Performing the trick with a non-standard deck of cards, with any number of suits and any number of cards in each suit, what is the probability of performing a successful magic trick?
<br><br>

Note:
<li>Assume that the deck is shuffled uniformly randomly.</li>
<li>Assume that any suit contains at least two cards, and every suit contains the king card and the queen card.</li>
<br><br>

A suit consists of  distinct cards numbered from <strong>1</strong> to <strong>C</strong>, and the cards numbered <strong>1</strong> and <strong>2</strong> are Kings and Queens respectively. Note that any card is uniquely identified by its suit and card number.

<br><br>

<h3>Input</h3>
The first line contains <strong>T</strong> denoting the number of test cases. Each of the next <strong>T</strong> lines consists of two space-separated integers <strong>S</strong> and <strong>C</strong>, denoting the number of suits and the number of cards in each suit respectively.
<br><br>

<h3>Constraints</h3>
<strong></strong><li><strong>1 ¡Ü T ¡Ü 1692 </strong>
<strong></strong></li><li><strong>1 ¡Ü S ¡Ü 36 </strong>
<strong></strong></li><li><strong>2 ¡Ü C ¡Ü 48 </strong>

<h3>Output</h3>
For each test case, print the probability of the magician performing a successful magic trick. An <strong>absolute</strong> error less than <strong>10<sup>-6</sup></strong> will be ignored.

<h3>Sample Input</h3>
<pre>2
2 2
2 3
</pre>

<h3>Sample Output</h3>
<pre>0.333333333333
0.133333333333
</pre>

<h3> Explanation</h3>
In the first test case, there are <strong>4</strong> cards in the deck (<strong>2</strong> suits with <strong>2</strong> cards each). This means that there can be <strong>4!</strong> different permutations of the shuffled cards. Only <strong>8</strong> of them contain at least one pair of adjacent Kings and Queens. The probability of a successful magic trick is, therefore, <strong>8/24 = 1/3</strong> 
<br><br>

<h3>Reference</h3>
<a href="https://www.hackerrank.com/contests/womens-codesprint-5/challenges/random-magic/problem">HackerRank - Random Magic</a>
</li>