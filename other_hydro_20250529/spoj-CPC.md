<p>Martin and Isa are very competitive. The newest competition they have created is about looking
at the plates of the cars. Each time one of them sees a car plate in the streets, he or she sends
to the other an SMS message with the content of that plate; the one who has seen the newest
plate is in the lead of the game. As the Automobile Car Management (ACM) office assigns the
plates sequentially in increasing order, they can compare them and find out who is the winner.

</p><p></p><p>
Martin has a very smart eye and he has stayed on the lead for several weeks. Maybe he keeps
looking at the streets instead of working, or maybe he stays all day in front of car selling
companies waiting for new cars to go out with new plates. Isa, tired of being always behind,
has written a program that generates a random plate, so the next time Martin sends a message
to her, she will respond with this generated plate. In this way, she hopes to give Martin a hard
time trying to beat her.

</p><p></p><p>
However, Martin has grown suspicious, and he wants to determine if Isa actually saw a car with
the plate she sent or not. This way, he will know if Isa is in the lead of the game.

</p><p></p><p>
He knows some facts about the plates assigned by the ACM:

</p><p></p><p>
</p><ul>
<li> Each plate is a combination of 7 characters, which may be uppercase letters (A-Z), or
digits (0-9).

<p></p><p>
</p></li><li> There exists two kinds of plate schemes: the old one, used for several years, and the new
one which has been in use for some months, when the combinations of the old one were
exhausted.

<p></p><p>
</p></li><li> In the old scheme, the first three characters were letters, and the last four were digits, so
the plates run from AAA0000 to ZZZ9999.

<p></p><p>
</p></li><li> In the new scheme, the first five characters are letters, and the last two are digits. Unfortunately
the chief of ACM messed up with the printing system while he was trying
to create a poster for his next campaign for mayor, and the printer is not able to write
the letters A, C, M, I, and P. Therefore, in this new scheme, the first plate is BBBBB00,
instead of AAAAA00.

<p></p><p>
</p></li><li> The plates are assigned following a sequential order. As a particular case, the last plate
from the old scheme is followed by the first plate from the new scheme.
</li></ul>

<p></p><p>
As Isa is not aware of all of this, she has just made sure that her random generator creates a
combination consisting of seven characters, where the first three characters are always uppercase
letters, the last two characters are always digits, and each one of the fourth and fifth characters
may be an uppercase letter or a digit (possibly generating an illegal combination, but she has
not much time to worry about that).

</p><p></p><p>
Of course, Martin will not consider Isa the winner if he receives an illegal combination, or if he
receives a legal plate, but equal to or older than his. But that��s not all of it. Since Martin knows
that new plates are not generated too fast, he will not believe that Isa saw a car with a plate
newer than the one he sent, but sequentially too far. For example, if Martin sends DDDDD45,
and receives ZZZZZ45, he will not believe that Isa saw a car with that plate, because he knows
that the ACM couldn��t have printed enough plates to get to ZZZZZ45 in the time he received
that answer.

</p><p></p><p>
So, Martin has decided to consider Isa the winner only if he receives a legal plate, newer than
his, and older than or equal to the C-th consecutive plate after the one he sent. He calls C his
confidence number. For example, if Martin sends ABC1234, and his confidence number is 6, he
will think that Isa is the winner only if he receives any plate newer than ABC1234, but older
than or equal to ABC1240.

</p><h3>Input</h3>
<p>The input contains several test cases. Each test case is described in a single line that contains
two strings S<sub>M</sub> and S<sub>I</sub> , and an integer C, separated by single spaces. S<sub>M</sub> is the 7-character
string sent by Martin, which is always a legal plate. S<sub>I</sub> is the 7-character string answered
by Isa, which was generated using her random generator. C is Martin��s <i>confidence number</i>
(1 &lt;= C &lt;= 10<sup>9</sup>).
The end of input is indicated by S<sub>M</sub> = S<sub>I</sub> =��*�� and C = 0.

</p><h3>Output</h3>
<p>For each test case, output a single line with the uppercase character ��Y�� if, according to Martin,
Isa is the winner, and with the uppercase character ��N�� otherwise.

</p><h3>Example</h3>

<pre><b>Input:</b>
ABC1234 ABC1240 6
ABC1234 ABC1234 6
ACM5932 ADM5933 260000
BBBBB23 BBBBC23 100
BBBBB23 BBBBD00 77
ZZZ9997 ZZZ9999 1
ZZZ9998 BBBBB01 3
ZZZZZ95 ZZZZZ99 10
BBBBB23 BBBBB22 5
* * 0

<b>Output:</b>
Y
N
N
N
Y
N
Y
Y
N
</pre>