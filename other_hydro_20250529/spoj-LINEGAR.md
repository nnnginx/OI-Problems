<p>&nbsp;</p>
<p><span style="font-size: medium;"> </span></p>
<pre>Ramesses II has just returned victorious from battle. To commemorate his
victory, he has decided to build a majestic garden. The garden will contain
a long line of plants that will run all the way from his palace at Luxor to
the temple of Karnak. It will consist only of lotus plants and papyrus
plants, since they symbolize Upper and Lower Egypt respectively.

The garden must contain exactly N plants. Also, it must be balanced: in any
contiguous section of the garden, the numbers of lotus and papyrus plants
must not differ by more than 2.

A garden can be represented as a string of letters ��L�� (lotus) and ��P��
(papyrus). For example, for N=5 there are 14 possible balanced gardens. In
alphabetical order, these are: LLPLP, LLPPL, LPLLP, LPLPL, LPLPP, LPPLL,
LPPLP, PLLPL, PLLPP, PLPLL, PLPLP, PLPPL, PPLLP, and PPLPL.

The possible balanced gardens of a certain length can be ordered
alphabetically, and then numbered starting from 1. For example, for N=5,
garden number 12 is the garden PLPPL.

TASK

Write a program that, given the number of plants N and a string that
represents a balanced garden, calculates the number assigned to this garden
modulo some given integer M. Note that for solving the task, the value of M
has no importance other than simplifying computations.

CONSTRAINTS

1 &lt;= N &lt;= 1,000,000
7 &lt;= M &lt;= 10,000,000

INPUT FORMAT:

* Line 1: N, the number of plants in the garden

* Line 2: M

* Line 3: A string of N characters ��L�� (lotus) or ��P�� (papyrus) that
        represents a balanced garden.

SAMPLE INPUT :

5
7
PLPPL

OUTPUT FORMAT:

* Line 1: Your program must write to the standard output a single line
        containing one integer between 0 and M-1 (inclusive), the
        number assigned to the garden described in the input, modulo
        M.

SAMPLE OUTPUT :

5

OUTPUT DETAILS:

The actual number assigned to PLPPL is 12. So, the output is 12 modulo 7,
which is 5.</pre>
<p>&nbsp;</p>