<p>With <a href="../BSMATH1/">your previous help</a>, Little Ben managed to get a perfect score on his homework. He came running home to show his brother, Big Ben. Big Ben had done this type of thing before, you see, so he naturally wasn't too impressed. Big Ben boasted, "Back in my day, we had to multiply and divide as well, the numbers were much bigger, AND we had to do it in base 64."</p>
<p>Little Ben became intrigued by this and searched the Internet for a worksheet. It turns out that his teacher made a worksheet for one of the higher grades that was just like Big Ben's. She also forgot to write what base each question was in... again!</p>
<p>According to the worksheet,</p>
<p style="padding-left: 30px; text-align: center;"><span style="font-family: 'courier new', courier;">The digits used for Base 64 are the same as that of Base 62, with the single- and double-quotes as the last two; the digits used are 0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz'".</span></p>
<p style="text-align: center;"><strong>Input</strong></p>
<p>The first line of input contains an integer <code>n</code> (1 &lt; n &lt; 64) that indicates the amount of sections (test cases). Each test case is as follows:</p>
<pre><span style="font-family: 'courier new', courier;">A - B = C
I
X1 op Y1 =
X2 op Y2 =
...
XI op YI =</span></pre>
<p>where <code>A - B = C</code> is the correct example, <code>I</code> (1 ¡Ü I ¡Ü 5000) is the number of questions in that section, <code>Xi</code> and <code>Yi</code> are the operands of each problem (0 &lt; X, Y ¡Ü 2<sup>100</sup>), and <code>op</code> is one of <br>[+, -, *, %], denoting addition, subtraction, multiplication, or modulo.</p>
<p style="text-align: center;"><br> <strong>Output</strong></p>
<p>Your program should output in the following format:</p>
<pre><span style="font-family: 'courier new', courier;">SECTION 1 (BASE b)<br>  X1 op Y1 = Z1<br>  X2 op Y2 = Z2<br>  ...<br>  Xi op Yi = Zi<br>SECTION 2 (BASE b)<br>  X1 op Y1 = Z1<br>  X2 op Y2 = Z2<br>  ...<br>  Xi op Yi = Zi<br>...<br>SECTION N (BASE b)<br>  X1 op Y1 = Z1<br>  X2 op Y2 = Z2<br>  ...<br>  Xi op Yi = Zi</span></pre>
<p>where <code>Zi</code> is the solution to <code>Xi op Yi</code>, and <code>b</code> is the base used. (2 ¡Ü b ¡Ü 64). <em>If the base is ambiguous, use the smallest base for which the example is correct and the questions are valid</em>.</p>
<p style="text-align: center;"><strong>Example</strong></p>
<p><strong>Input:</strong></p>
<pre style="color: #000000; font-family: Verdana, Arial, Helvetica, sans-serif; font-size: 10px; margin: 8px;"><span style="font-size: x-small;"><span style="font-size: small;"><span style="font-family: 'courier new', courier;">4
K72Q - 9C5U = APRR
3
11JH4 - BMEB =
PB04 % DQ9O =
F0GM - UQR0 =
A654A - 9A60E = AE3B
2
B94BA + 3460A =
123A29 % 5E065 =
37CR - olh = 2KSm
5
157W % 1bIJ =
1P56 % 1Eob =
1C6I * 1"uX =
1Ktc % 1BMf =
20ne * 22V" =
BQfC -</span><span style="font-family: 'courier new', courier;"> 4Kdb = 761H
2</span></span><span style="font-size: small;"><span style="font-family: 'courier new', courier;">
9aFL * 3WU3 =
5fc</span></span><span style="font-size: small;"><span style="font-family: 'courier new', courier;">V + 7fWL =</span></span></span></pre>
<p><strong>Output:</strong></p>
<pre style="color: #000000; font-family: Verdana, Arial, Helvetica, sans-serif; font-size: 10px; margin: 8px;"><span style="font-size: small;"><span style="font-family: 'courier new', courier;">SECTION 1 (BASE 31)
  11JH4 - BMEB = KS2O
  PB04 % DQ9O = BFLB
  F0GM - UQR0 = -FQA9
SECTION 2 (BASE 15)
  B94BA + 3460A = EDAC5
  123A29 % 5E065 = 5594E
SECTION 3 (BASE 64)
  157W % 1bIJ = 157W
  1P56 % 1Eob = AIX
  1C6I * 1"uX = 2O3gS"I
  1Ktc % 1BMf = 9Wz
  20ne * 22V" = 46bA3EO
SECTION 4 (BASE 42)
  9aFL * 3WU3 = bBafS</span></span><span style="font-size: small;"><span style="font-family: 'courier new', courier;">4L
  5fcV + 7fWL = DfTA</span></span></pre>
<p style="text-align: center;"><strong>Notes: large input/output data</strong></p>