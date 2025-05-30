<p>A group of Jedi Knights is having a competition. One of the Knights at random stands
within a circle. The other Knights, in a random order, challenge him. If a challenger de-
feats the Knight of the Round Circle, that Knight must leave the contest. The challenger
then becomes the new Knight of the Round Circle and, as such, will face all subsequent
challengers until he is defeated. If the current Knight of the Round Circle wins the chal-
lenge, he stays within the circle and the challenger must leave the competition. The Knight
within the circle at the end of the competition is deemed the winer. You may assume that
no two Knights have exactly the same skill and that a stronger Knight will always defeat
a weaker Knight.<br><br>
Suppose there are three Knights in the competition. If the strongest one happens to stand
in the circle first, he will not be defeated, so no one will ever leave the circle. If the weakest
one happens to be first in the circle, he will be kicked out after his first match. If th e
Knight that defeated him was the strongest, he will win the final challenge as well (so only
one Knight will ever leave the circle),otherwise the strongest Knight will kick the middle
Knight out of the circle during his challenge (so that two Knights leave the circle). If the
middle Knight stands in the circle first, he will be the only one kicked out of the circle, no
matter what order the other two come at him. All in all, an average of 5/6 or 0.83 Knight
will leave the circle during the competition.<br><br>
You are to compute the average number of Knights to leave the circle during a competition
given the number of Knights in the competition.


</p><h3>Input</h3>
<p>The input consists of several lines. Each line (but the last) will contain one positive decimal
integer no larger than 10000. This integer is followed by exactly one <eol>. These integers
represent the number of Knights in the competition. The last line will contain one zero,
followed by <eol>. This line is not to be processed; it merely signifies the end of the input.


</eol></eol></p><h3>Output</h3>
<p>The output cases are to appear in the same order in wich they appear in the input. For
each case, you are to print With c competitors, a Jedi Knight will be replaced
approximately t times. c is the number of competitors in this case and should be a
decimal integer. t is the average number of times a Jedi Knight leaves the circle and
should be a floating point decimal number with exactly two digits following the decimal
point. There should always be at least one digit before the decimal point (use 0.50 rather
.50, for example) The statement should be followed by two <eol>��s, wich is to say that a
blank line should follow every output case.


</eol></p><h3>Example</h3>

<pre><b>Input:</b>
3
1000
0

<b>Output:</b>
With 3 competitors, a Jedi Knight will be replaced approximately 0.83 times.

With 1000 competitors, a Jedi Knight will be replaced approximately 6.49 times.

</pre>