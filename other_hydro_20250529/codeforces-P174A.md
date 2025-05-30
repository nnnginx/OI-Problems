## Description

<div><p>A group of <span class="tex-span"><i>n</i></span> merry programmers celebrate Robert Floyd's birthday. Polucarpus has got an honourable task of pouring Ber-Cola to everybody. Pouring the same amount of Ber-Cola to everybody is really important. In other words, the drink's volume in each of the <span class="tex-span"><i>n</i></span> mugs must be the same.</p><p>Polycarpus has already began the process and he partially emptied the Ber-Cola bottle. Now the first mug has <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> milliliters of the drink, the second one has <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> milliliters and so on. The bottle has <span class="tex-span"><i>b</i></span> milliliters left and Polycarpus plans to pour them into the mugs so that the main equation was fulfilled.</p><p>Write a program that would determine what volume of the drink Polycarpus needs to add into each mug to ensure that the following two conditions were fulfilled simultaneously: </p><ul> <li> there were <span class="tex-span"><i>b</i></span> milliliters poured in total. That is, the bottle need to be emptied; </li><li> after the process is over, the volumes of the drink in the mugs should be equal. </li></ul></div><div class="input-specification"><p>The first line contains a pair of integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>b</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100, 1 ≤ <i>b</i> ≤ 100</span>), where <span class="tex-span"><i>n</i></span> is the total number of friends in the group and <span class="tex-span"><i>b</i></span> is the current volume of drink in the bottle. The second line contains a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the current volume of drink in the <span class="tex-span"><i>i</i></span>-th mug.</p></div><div class="output-specification"><p>Print a single number "<span class="tex-font-style-tt">-1</span>" (without the quotes), if there is no solution. Otherwise, print <span class="tex-span"><i>n</i></span> float numbers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the volume of the drink to add in the <span class="tex-span"><i>i</i></span>-th mug. Print the numbers with no less than 6 digits after the decimal point, print each <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> on a single line. Polycarpus proved that if a solution exists then it is unique.</p><p>Russian locale is installed by default on the testing computer. Make sure that your solution use the point to separate the integer part of a real number from the decimal, not a comma.</p></div>


## Input

<p>The first line contains a pair of integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>b</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100, 1 ≤ <i>b</i> ≤ 100</span>), where <span class="tex-span"><i>n</i></span> is the total number of friends in the group and <span class="tex-span"><i>b</i></span> is the current volume of drink in the bottle. The second line contains a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the current volume of drink in the <span class="tex-span"><i>i</i></span>-th mug.</p>


## Output

<p>Print a single number "<span class="tex-font-style-tt">-1</span>" (without the quotes), if there is no solution. Otherwise, print <span class="tex-span"><i>n</i></span> float numbers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the volume of the drink to add in the <span class="tex-span"><i>i</i></span>-th mug. Print the numbers with no less than 6 digits after the decimal point, print each <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> on a single line. Polycarpus proved that if a solution exists then it is unique.</p><p>Russian locale is installed by default on the testing computer. Make sure that your solution use the point to separate the integer part of a real number from the decimal, not a comma.</p>


## Samples

```input1
5 50
1 2 3 4 5

```

```output1
12.000000
11.000000
10.000000
9.000000
8.000000

```






```input2
2 2
1 100

```

```output2
-1

```



