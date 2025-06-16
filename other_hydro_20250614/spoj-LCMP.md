<p><strong>N</strong> Slovakistan farmers own neighbouring fields alongside a river, forming a straight line. Each field is infested with (possibly zero) pests.</p>
<p>Thanks to ingenious Slovakistan science, each species of pest can be assigned a prime number. Each field can then be assigned a positive number, representative of the pests that are infesting it - the prime factorization of this number indicates which pests are present, with the powers of each prime number representing how strongly the field is infested with that pest.</p>
<p>Every pesticide can then be assigned a positive number, which is designed in such a way that its prime factorization indicates what pests it can supress, with the powers of each prime number representing how strong infestations of that pest it is able to handle.</p>
<p>To aid their farmers, the government of Slovakistan can select a pest, and then pump a pesticide designed specifically against it into the river, completely supressing that species on all fields. However, due to environmental concerns, they will only use one pesticide at a time - when the government switches to a different pesticide, designed against a different pest, the ones previously supressed return to all fields in full force.</p>
<p>On top of that, the farmers union can request pesticide to be sprayed on the fields themselves. Since this is done using an airplane, they can only request pesticide to be sprayed on a contiguous segment of fields.</p>
<p>Pesticides with higher numbers are more expensive. Now, for each request the government would like to know the cheapest pesticide they can use to supress all pests on all the fields in the requested segment.</p>
<h3>Input</h3>
<p>The first line contains two integers <strong>1 ¡Ü&nbsp;N ¡Ü&nbsp;50000 </strong>and <strong>1 ¡Ü&nbsp;Q&nbsp; ¡Ü 10<sup>5</sup>&nbsp;</strong>- the number of fields and the number of events.</p>
<p>The second line contains <strong>N</strong> integers <strong>f<sub>1</sub></strong>, ..., <strong>f<sub>N</sub></strong>&nbsp;- the numbers assigned to the fields. They will be positive and not greater than <strong>10<sup>5</sup></strong>.</p>
<p><strong> Q</strong> lines follow, describing events in the order in which they happened. Each event is either of the form <strong>0 L R</strong> or <strong>1 P</strong>.</p>
<p>If the event is of the form <strong>1 P</strong>, <strong>1 ¡Ü P ¡Ü 10<sup>5</sup></strong>, it means that the government of Slovakistan began pumping pesticide against the pest number <strong>P</strong> (a prime number) into the river, and are no longer pumping pesticide against the previous pest, if they were doing so. The exception is <strong>P = 1</strong>, meaning that there is simply no pesticide being pumped into the river. In the beginning, the government is not pumping any pesticide.</p>
<p>If the event is of the form <strong>0 L R</strong>,<strong> 1 ¡Ü L ¡Ü&nbsp;R ¡Ü N</strong>, it means that the farmers requested pesticide to be sprayed on the contiguous segment of fields from the <strong>L</strong>-th to the <strong>R</strong>-th, inclusive.</p>
<h3>Output</h3>
<p>For each event of form&nbsp;<strong>0 L R</strong>, output the smallest number of pesticide which can handle all infestations on the segment of fields from <strong>L</strong> to <strong>R</strong>, modulo <strong>10<sup>9</sup>+7</strong>, taking into account that some pests may be supressed due to the government's aid. More formally, output the least common multiple of the numbers <strong>f<sub>L</sub></strong>, ..., <strong>f<sub>R</sub></strong>, after they have had all factors of <strong>P </strong>from the last <strong>1 P</strong>&nbsp;event removed, modulo <strong>10<sup>9</sup>+7</strong>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
10 12
4 2 3 5 6 47 10007 32768 59049 1
0 1 5
0 2 5
1 2
0 1 5
0 2 5
0 6 10
1 3
0 6 10
1 1
0 1 10
0 10 10
0 1 5

<strong>Output:</strong>
60
30
15
15
772456932
411740567
342852967
1
60</pre>