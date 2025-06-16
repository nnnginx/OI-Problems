<p>
<img src="/content/simba:p6.jpg" style="float: right" vspace="3" hspace="8" alt="Illustration">

Luke Skywalker successfully leads the rebel starship fleet to break the Emperor's siege of the planet Endor. The rebels, jubilant in their victory, return to their base on the moon of Endor to pay their homage to Princess Leia. They fly towards the parking bay where there are n parking slots in a row. One by one n starships numbered S<sub>1</sub> to S<sub>n</sub> enter the parking bay. Each rebel R<sub>i</sub> heads to his favorite parking slot P<sub>i</sub>, and if it is free, he docks his starship there. Otherwise, he continues further to the next free slot and occupies it. But if all succeeding slots are occupied, he leaves for good. How many sequences P<sub>i</sub> are such that every rebel can dock his starship?

</p><h3>Input Description</h3>
<p>
The first line of the input is a positive integer t ¡Ü 20, which is the number of test cases. The descriptions of the test cases follow one after the other. The description of each test case contains exactly one line (a positive integer), containing the value of n ¡Ü 1000000.

</p><h3>Output Description</h3>
<p>
The output consists of exactly t lines. The ith line should be A<sub>i</sub>%10007, where A<sub>i</sub> is the number of sequences in the i<sup>th</sup> case, and 'x%y' represents the remainder when x is divided by y.

</p><h3>Example</h3>
<p>
<br><b>Input<br></b>

2<br>
1<br>
2<br>

<br><b>Output<br></b>
1<br>
3

<br><br><b>Explanation</b>: In the given example, 11, 12 and 21 are the possible sequences.

</p>