<p>A new web-design studio, called SMART (Simply Masters of ART), employs two people. The first one is a web-designer and an executive director at the same time. The second one is a programmer. The director is so a nimble guy that the studio has already got <b>N</b> contracts for web site development. Each contract has a deadline <b>d<sub>i</sub></b>.

</p><p>It is known that the programmer is lazy. Usually he does not work as fast as he could. Therefore, under normal conditions the programmer needs <b>b<sub>i</sub></b> of time to perform the contract number <b>i</b>. Fortunately, the guy is very greedy for money. If the director pays him <b>x<sub>i</sub></b> dollars extra, he needs only <b>(b<sub>i</sub> - a<sub>i</sub>*x<sub>i</sub>)</b> of time to do his job. But this extra payment does not influence other contracts. This means that each contract should be paid separately to be done faster. The programmer is so greedy that he can do his job almost instantly if the extra payment is <b>(b<sub>i</sub>/a<sub>i</sub>)</b> dollars for the contract number <b>i</b>.

</p><p>The director has a difficult problem to solve. He needs to organize programmer¡¯s job and, may be, assign extra payments for some of the contracts so that all contracts are performed in time. Obviously he wishes to minimize the sum of extra payments. Help the director!

</p><h3>Input</h3>
<p>First line of the input contains an integer <b>t</b> (<i>1</i> ¡Ü <b>t</b> ¡Ü <i>45</i>), equal to the number of testcases. Then descriptions of <b>t</b> testcases follow.

</p><p>First line of description contains the number of contracts <b>N</b> (<i>1</i> ¡Ü <b>N</b> ¡Ü <i>100000</i>, integer). Each of the next <b>N</b> lines describes one contract and contains integer numbers <b>a<sub>i</sub></b>, <b>b<sub>i</sub></b>, <b>d<sub>i</sub></b> (<i>1</i> ¡Ü <b>a<sub>i</sub></b>, <b>b<sub>i</sub></b> ¡Ü <i>10000</i>; <i>1</i> ¡Ü  <b>d<sub>i</sub></b> ¡Ü <i>1000000000</i>) separated by spaces.

</p><p>At least <i>90%</i> of testcases will have <i>1</i> ¡Ü <b>N</b> ¡Ü <i>10000</i>.

</p><h3>Output</h3>
<p>For each testcase in the input your program should output one line with a single real number S. Here S is the minimum sum of money which the director needs to pay extra so that the programmer could perform all contracts in time. The number must have two digits after the decimal point.

</p><h3>Example</h3>

<pre><b>Input:</b>
1
2
20 50 100
10 100 50

<b>Output:</b>
5.00
</pre>